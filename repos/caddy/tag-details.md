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
$ docker pull caddy@sha256:abf97331ba731afdbe77aafef9738f37f5073739ad99cdced920c974c73ca4f4
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
$ docker pull caddy@sha256:629c5800ccf51df482a4e63266e4570de3e573e862d902398b03cbfca2212b4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e073d63a624f18bd8e2f94b9e84715e5a33a817db19afa42afc8ea95e59d568`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:17 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:24 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc82ca1670c70e5b605729b271409acba02ca26c3f669bf1d95a067fb853a90`  
		Last Modified: Thu, 01 Apr 2021 13:54:20 GMT  
		Size: 300.0 KB (300021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d66f69260e9358ba74c27e0ed110b9ff7781c5f90d5d01f86d6ef289834382`  
		Last Modified: Thu, 01 Apr 2021 13:54:17 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b38557b1fd80a7712b7263f0896f076afdeb9f25f68a79e288b87490aa3047`  
		Last Modified: Thu, 01 Apr 2021 13:54:19 GMT  
		Size: 11.6 MB (11622380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37d6fba45d5f1633f00b6a9d204abacad2a6918dc355706fe0decc0bc4e565`  
		Last Modified: Thu, 01 Apr 2021 13:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b57cdc61b54865a7ff2ea4ef9d16458537d40e0dc25559d6540111874abbe4ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88293e19906b6b2275ff6e127e29960b1fdf0cf0c4baa4bbce4ea297e90db731`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:36:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:36:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:36:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 17:36:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:36:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:36:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:36:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:36:56 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 17:36:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:36:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:37:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:37:07 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:37:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:37:10 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:37:11 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:37:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1532456df32c320ccd3c9ff5433c9e44d873ef87a0dc9fc29f9cf256b517eb4`  
		Last Modified: Wed, 31 Mar 2021 17:38:50 GMT  
		Size: 300.1 KB (300103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263f61714ef61a0c59bef8e70bc49a741a357b0a0fc556b44f8344df37ea0f8`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818002dab28746359de43d5a88d06c77cc3a353c838e15c6b6a67d48352cc5c0`  
		Last Modified: Wed, 31 Mar 2021 17:38:54 GMT  
		Size: 10.9 MB (10944835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979a3c808bf5c07c668f5966a15458dbfe9aba5aa7d761e690dd3a5cadf45eb`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6d510324512c20fc0d40aeb8b6e5b98255c857ad2dee894b6cb6e66f0231cf9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42db38da968682707e6cf0fabb16f93770388907d8a208fca0db74cae3183ba2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:11:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:11:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:11:48 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 08:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:11:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:11:56 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:11:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:11:58 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:11:59 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 08:12:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:12:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:12:09 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:12:11 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:12:13 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:12:15 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:12:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547b5d01ba24abc02b4f05f8134bfb156ce1840f496ed03a1316c882625bd41f`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 299.2 KB (299199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a883a914d37801ae97b0fac82c62e4f70ef4c92fc53417a91a23b2e69d36d9bb`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475143e7b89d1a36700916ec3c8f0caae9b57d5cd9ba187b9f3fd5d9a71eddcf`  
		Last Modified: Thu, 01 Apr 2021 08:13:38 GMT  
		Size: 10.9 MB (10925346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79cdab22a3397c4a98f63a7e96c51881033744b1f198c4984072e7303e9f73`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1c3e6c1b947162789190f9215b56c517caa5c48bd5d09f9753c6ff105ece8ea4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d36a254c95d4ad655ca159d67b79ad8ca4498f82a3c127340a7b5be09e213b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:40:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:40:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:40:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 12:40:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:40:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:40:35 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:40:38 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:40:44 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:40:49 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:40:53 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 12:40:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:40:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:40:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:40:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:40:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:41:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:41:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:41:05 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:41:08 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:41:12 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:41:18 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1fbebcb85e1b4f7457195688308678e46184f78ec8402dcd4eb0992700541`  
		Last Modified: Thu, 01 Apr 2021 12:45:24 GMT  
		Size: 300.3 KB (300333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c34c85964e1be21b929d726522dfd448c029aaf7acd32bf5342ff93070124bd`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c657d5761128c010be222b8ddea92ceba700a3c76afb7704c9d436bbb5582c1`  
		Last Modified: Thu, 01 Apr 2021 12:45:27 GMT  
		Size: 10.6 MB (10598978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90c89f24747de4d19b1c83875e0072662bfe7ce4c5f4e15c551d907b212ebc`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:d8ff14acdf013e9a2df27d95f3326bf7175307a04e9e6f7a40b840bf813898ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63b8a5e4185f59e46edc1e47b15d592327b0c3b8867d3edd3be3a9b3dea5522`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:49:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:49:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:49:51 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:50:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:50:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:50:24 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:50:30 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:50:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 05:50:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:50:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:50:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:50:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:50:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:51:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:51:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:51:24 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:51:30 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:51:35 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:51:40 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:51:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69ab62cc22d6fb5ba7a45731c0b8f378026c7c711d7d48946bfe7c69eae199`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 302.3 KB (302337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9767f7d2aec64fa7c89aa12c9b2b14b03dbe10e20cf53279a88f5009dd2c7841`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502018de7a2dcf0f08830ebcce7c073c9a9db95ecf366d96d44c7a76ba032edc`  
		Last Modified: Fri, 26 Mar 2021 05:58:02 GMT  
		Size: 10.2 MB (10241383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61815e7304b64383c90b6c68c7220f40b74c932f3dd3cfd44b04fed05920aec`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:9d992badb7530225182676af12ae945f5f2de2f5ad7d3946b397892a6de4c123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c8a68869d0806c29e6c2c9c655d3e9085af285c6c24ea651ad3bdffd714e38`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:55:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:00 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:05 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:06 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:08 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8eb19b6319d0b09121581759094c3eb58e5574e2063affb6c42c0e1a1937a0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd6e269a873b8a21e2787b0ea05662c0f2676aa9043f52b8884081965be7112`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f6a8a7e19cb11edbda771ce361181202915f4760cdaef5e290b1758cc7b88c`  
		Last Modified: Wed, 31 Mar 2021 18:57:02 GMT  
		Size: 11.3 MB (11272066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec92d2dcab4ee41e4e626d8b360a6feff3822db894894865a36bbe9cfc759df0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:a18e9c84fb32bae7eeaab4b048f10c4ec8797e4641f8d7d5f75d35e11282d0e3
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
$ docker pull caddy@sha256:629c5800ccf51df482a4e63266e4570de3e573e862d902398b03cbfca2212b4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e073d63a624f18bd8e2f94b9e84715e5a33a817db19afa42afc8ea95e59d568`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:17 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:24 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc82ca1670c70e5b605729b271409acba02ca26c3f669bf1d95a067fb853a90`  
		Last Modified: Thu, 01 Apr 2021 13:54:20 GMT  
		Size: 300.0 KB (300021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d66f69260e9358ba74c27e0ed110b9ff7781c5f90d5d01f86d6ef289834382`  
		Last Modified: Thu, 01 Apr 2021 13:54:17 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b38557b1fd80a7712b7263f0896f076afdeb9f25f68a79e288b87490aa3047`  
		Last Modified: Thu, 01 Apr 2021 13:54:19 GMT  
		Size: 11.6 MB (11622380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37d6fba45d5f1633f00b6a9d204abacad2a6918dc355706fe0decc0bc4e565`  
		Last Modified: Thu, 01 Apr 2021 13:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b57cdc61b54865a7ff2ea4ef9d16458537d40e0dc25559d6540111874abbe4ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88293e19906b6b2275ff6e127e29960b1fdf0cf0c4baa4bbce4ea297e90db731`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:36:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:36:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:36:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 17:36:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:36:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:36:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:36:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:36:56 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 17:36:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:36:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:37:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:37:07 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:37:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:37:10 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:37:11 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:37:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1532456df32c320ccd3c9ff5433c9e44d873ef87a0dc9fc29f9cf256b517eb4`  
		Last Modified: Wed, 31 Mar 2021 17:38:50 GMT  
		Size: 300.1 KB (300103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263f61714ef61a0c59bef8e70bc49a741a357b0a0fc556b44f8344df37ea0f8`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818002dab28746359de43d5a88d06c77cc3a353c838e15c6b6a67d48352cc5c0`  
		Last Modified: Wed, 31 Mar 2021 17:38:54 GMT  
		Size: 10.9 MB (10944835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979a3c808bf5c07c668f5966a15458dbfe9aba5aa7d761e690dd3a5cadf45eb`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6d510324512c20fc0d40aeb8b6e5b98255c857ad2dee894b6cb6e66f0231cf9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42db38da968682707e6cf0fabb16f93770388907d8a208fca0db74cae3183ba2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:11:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:11:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:11:48 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 08:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:11:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:11:56 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:11:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:11:58 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:11:59 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 08:12:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:12:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:12:09 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:12:11 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:12:13 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:12:15 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:12:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547b5d01ba24abc02b4f05f8134bfb156ce1840f496ed03a1316c882625bd41f`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 299.2 KB (299199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a883a914d37801ae97b0fac82c62e4f70ef4c92fc53417a91a23b2e69d36d9bb`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475143e7b89d1a36700916ec3c8f0caae9b57d5cd9ba187b9f3fd5d9a71eddcf`  
		Last Modified: Thu, 01 Apr 2021 08:13:38 GMT  
		Size: 10.9 MB (10925346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79cdab22a3397c4a98f63a7e96c51881033744b1f198c4984072e7303e9f73`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1c3e6c1b947162789190f9215b56c517caa5c48bd5d09f9753c6ff105ece8ea4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d36a254c95d4ad655ca159d67b79ad8ca4498f82a3c127340a7b5be09e213b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:40:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:40:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:40:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 12:40:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:40:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:40:35 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:40:38 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:40:44 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:40:49 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:40:53 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 12:40:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:40:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:40:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:40:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:40:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:41:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:41:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:41:05 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:41:08 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:41:12 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:41:18 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1fbebcb85e1b4f7457195688308678e46184f78ec8402dcd4eb0992700541`  
		Last Modified: Thu, 01 Apr 2021 12:45:24 GMT  
		Size: 300.3 KB (300333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c34c85964e1be21b929d726522dfd448c029aaf7acd32bf5342ff93070124bd`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c657d5761128c010be222b8ddea92ceba700a3c76afb7704c9d436bbb5582c1`  
		Last Modified: Thu, 01 Apr 2021 12:45:27 GMT  
		Size: 10.6 MB (10598978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90c89f24747de4d19b1c83875e0072662bfe7ce4c5f4e15c551d907b212ebc`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d8ff14acdf013e9a2df27d95f3326bf7175307a04e9e6f7a40b840bf813898ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63b8a5e4185f59e46edc1e47b15d592327b0c3b8867d3edd3be3a9b3dea5522`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:49:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:49:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:49:51 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:50:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:50:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:50:24 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:50:30 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:50:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 05:50:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:50:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:50:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:50:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:50:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:51:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:51:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:51:24 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:51:30 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:51:35 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:51:40 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:51:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69ab62cc22d6fb5ba7a45731c0b8f378026c7c711d7d48946bfe7c69eae199`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 302.3 KB (302337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9767f7d2aec64fa7c89aa12c9b2b14b03dbe10e20cf53279a88f5009dd2c7841`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502018de7a2dcf0f08830ebcce7c073c9a9db95ecf366d96d44c7a76ba032edc`  
		Last Modified: Fri, 26 Mar 2021 05:58:02 GMT  
		Size: 10.2 MB (10241383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61815e7304b64383c90b6c68c7220f40b74c932f3dd3cfd44b04fed05920aec`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9d992badb7530225182676af12ae945f5f2de2f5ad7d3946b397892a6de4c123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c8a68869d0806c29e6c2c9c655d3e9085af285c6c24ea651ad3bdffd714e38`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:55:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:00 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:05 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:06 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:08 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8eb19b6319d0b09121581759094c3eb58e5574e2063affb6c42c0e1a1937a0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd6e269a873b8a21e2787b0ea05662c0f2676aa9043f52b8884081965be7112`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f6a8a7e19cb11edbda771ce361181202915f4760cdaef5e290b1758cc7b88c`  
		Last Modified: Wed, 31 Mar 2021 18:57:02 GMT  
		Size: 11.3 MB (11272066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec92d2dcab4ee41e4e626d8b360a6feff3822db894894865a36bbe9cfc759df0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:803eb2fbf7bc2389c531d241d9596982a84cb74a9d37fc2659e95c3f8ebeccaf
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
$ docker pull caddy@sha256:a9cf52bbabc8864aa2bb39cc3b30034060f8b5cfea57a24af5d59fb712a2363d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119514478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972e1302f4350651067d073928bc15bcd5b0219ea111332de1bb9a3eb2af6800`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:14:43 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:14:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:14:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:18:53 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 20:20:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:20:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:20:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:20:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:20:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbbf235a55c104bafc6765f3c92a36489a596041551360d566152f2af01b59`  
		Last Modified: Wed, 31 Mar 2021 20:22:25 GMT  
		Size: 280.9 KB (280881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f184a059628efa0b05f924f5b1e223377ebd57cdec0597912aabcd4b2129b`  
		Last Modified: Wed, 31 Mar 2021 20:23:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec81731eed009f8d947489208d3bc2fe161411bd6ad9543fc2af27bb229d352`  
		Last Modified: Wed, 31 Mar 2021 20:26:05 GMT  
		Size: 106.8 MB (106811699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec2af768a6dad08fb2f9bf5396591d7ab1b7bff816d42c96f7c5169ab05502`  
		Last Modified: Wed, 31 Mar 2021 20:25:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d41b37a714ddeeea16e8fb5e39787ea218dc37873bcc66c101e72177214f54`  
		Last Modified: Thu, 01 Apr 2021 13:54:35 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30dccfb57aae7671a60a9a97a865cdfb7223a51d8d176ca6c833f95a3d0c3`  
		Last Modified: Thu, 01 Apr 2021 13:54:36 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c224dde9c00bfc5be3cc063759e6e39bb2d1586ad856299e4dc5edcbce99ea0d`  
		Last Modified: Thu, 01 Apr 2021 13:54:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:528de32f232e1620d7a832171f2de05db14a38b0367b601508a3554ee39609d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cb88e37729e6535c0e5d37dd52aabf2191db2fc10d3a2d5cc2befb4a3547e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:45:17 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:45:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:45:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:13:42 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 19:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 19:21:40 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 19:21:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 19:21:45 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:04:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:00 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:02 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 04:05:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa6796eed51884cd0436f134281af9489342ecf256aec0b31ca83f254ccd0d1`  
		Last Modified: Wed, 31 Mar 2021 19:23:16 GMT  
		Size: 281.0 KB (280979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c043dc86373f816c29db582d9bddada9a00eeb3812a357a2dfd8e3f68d9a413`  
		Last Modified: Wed, 31 Mar 2021 19:23:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031875ceeaab9b0b96a47b7ed9ec2a0098a9d8662d1c2a57785eb95dbf36d419`  
		Last Modified: Wed, 31 Mar 2021 19:25:23 GMT  
		Size: 102.7 MB (102671786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15870044ac3cd6474d13a6fd94871020ad8801d56fa4387bb9507968da9b093d`  
		Last Modified: Wed, 31 Mar 2021 19:24:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa970c15af3c0912614e0bd697d3329aa1d7f2e98e13f86227bec493367295`  
		Last Modified: Thu, 01 Apr 2021 04:06:04 GMT  
		Size: 7.9 MB (7929419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231389672c1c8c7a9fd39092006eca8983b058e9edc5f0d04bf43bc3f9dea700`  
		Last Modified: Thu, 01 Apr 2021 04:06:02 GMT  
		Size: 1.2 MB (1221595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efaab869ceebc633c179dc051159fb587f7bb30890e765be3f630558cc9933c`  
		Last Modified: Thu, 01 Apr 2021 04:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:673ccce087f4fef545f63f971a0738dbb551fa5872c1742be37a89daded09f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83363f4d6122099578251753b8d8052a348737a2593393b43b431795fcb64292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:56:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:56:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:56:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:36:58 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 01 Apr 2021 12:59:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 12:59:20 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 12:59:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:59:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 12:59:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:27 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 14:30:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:30:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b725919da0175e4c01c41441c29fff6f5ec6c0c4e37417f70120f08f96acfc`  
		Last Modified: Thu, 01 Apr 2021 13:01:16 GMT  
		Size: 280.1 KB (280073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1f51d8714e34d5e746102b7176e77e8142ecf71f4c68d82354285a0bd6d16`  
		Last Modified: Thu, 01 Apr 2021 13:01:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9a84aba5c985724e2f9d0049434534ed654c74b46945f50cc2af08567b9b6`  
		Last Modified: Thu, 01 Apr 2021 13:03:20 GMT  
		Size: 102.5 MB (102462580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc655d7de77ca2ce887998caba1ec52a0bd3f8aa5453bb583ba83449613e96c5`  
		Last Modified: Thu, 01 Apr 2021 13:02:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c177cdf044a6b683b9c1a95121917806970172353334871227cb79e618bc0b1`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1d6a25abce1b9f81c345e1c2ac0149a173ffdcdca04c5ffd9a450903aa2d2`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 1.2 MB (1219450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1bc2f6f317df593b6011ce90f58a1234127d7f78cf8121f8972f79d564b69`  
		Last Modified: Thu, 01 Apr 2021 14:31:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e8c8a0956ea40a17133ef7055aa4cd1076f944342cddf3665d91c8addbe8effb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8892c660131d71ee38d69f56f72c5e98aed80471af824bd1ceda7b5a08c2ce4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:51:33 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:57:28 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:00:54 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:01:02 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:11:38 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 16:11:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:11:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:11:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:11:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f941853f4c183d3b0a653353ba7515088ae2488b01a0ca6bddaa6f1dcc062d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 281.2 KB (281215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4be3bf1d235e013412b55ba1e824da6cfebaf80d284481002d2aa00718563d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc4f0c823675028e8e8caed39be27c63850615a4394ab508faf5b4ed3a9fc3`  
		Last Modified: Fri, 26 Mar 2021 01:04:37 GMT  
		Size: 102.1 MB (102143643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ce0d84f3cb43a1eb06c18a87965b988275ab2c863043b96032d5d4b94d5db`  
		Last Modified: Fri, 26 Mar 2021 01:04:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6274beb5e6ef4051612c2bcfadde952a3caceb7145e9f6d61ce0b818f2e4f7`  
		Last Modified: Fri, 26 Mar 2021 16:12:33 GMT  
		Size: 8.5 MB (8500012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880cf9840fe472a748b59dbd60483c321b780ac76a1906aafe3c082bfd41496d`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 1.2 MB (1201557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d154a0032206067bed60392933ce1a8bab8e7cd48226b92f0f589d7f1bd746`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:b84ae4910f796380e57d7daac89af75d8012094746a88fa467d97bafcdb11fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113985368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b7945ba534d20ab228061857652036740c946d79102221e87b9fb0ea979254`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:50:54 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:58:55 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:01:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:01:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:01:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:02:00 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:52:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:52:17 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:52:23 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:52:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:52:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:52:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22fc023a51f1560551f97595c0d26436968276b81fd2119cb972238aff23fb6`  
		Last Modified: Fri, 26 Mar 2021 01:06:49 GMT  
		Size: 283.2 KB (283209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b5b049d7abfca6a07577171113a612a55eb6f864651563d204b02fb5c4e60`  
		Last Modified: Fri, 26 Mar 2021 01:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db853427f2ec5049b1f9079b25be4c8117deaa1fcac132410fa8c0b1deb720c8`  
		Last Modified: Fri, 26 Mar 2021 01:12:48 GMT  
		Size: 100.8 MB (100803535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d927b70afd72e9dd133e5d57a45143c8e8ebceefa2dfc3a7fc1bd8e1b9ce83d8`  
		Last Modified: Fri, 26 Mar 2021 01:12:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf5bc1fa9c61f972e646bacb633a53efd7d173b4d79b2efd32f923d503d50b`  
		Last Modified: Fri, 26 Mar 2021 05:58:21 GMT  
		Size: 8.9 MB (8921440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6874c8aee6bfafc6a12719998f12ce1dcf70d8a61da3dd914f9c791808221`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0826f628855fe686aafb0d3423a1c5258fcb72287998561865187f7e7d4f0`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:e7648a8c6fc41f80b2eb8da973742a7485f479cb4f57dcb04d738e8800f5b64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118389839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8b0338c771c7f370f6460e6a444505905acc419685f5c8d35648800e50d8c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:34:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:34:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:34:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:38:18 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 18:39:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:39:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:39:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:39:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:39:47 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:15 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb296d6fc71cd9057e3d03d0ea4ebe30a620f7c6ce57eb78f4c137e77a9a47`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 281.4 KB (281355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783b7db1c405d51f50a261ae252c97941c44ffeb93cb10c2e2bdd458296774a`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb58064707977215f9632cdb206eaec9d63534f602e5682c22634dcfbb2cbd5`  
		Last Modified: Wed, 31 Mar 2021 18:42:02 GMT  
		Size: 105.9 MB (105923109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273a64a6b34c09c3baa0d7e2dc15a36980a72e658c1570903625ebac61f7f16`  
		Last Modified: Wed, 31 Mar 2021 18:41:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadae105e5bbdd611f262c9d81668d5b3251f7c246bd9bd444ecd4c88b936326`  
		Last Modified: Wed, 31 Mar 2021 18:57:12 GMT  
		Size: 8.4 MB (8352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7739fc64956105cdc380f5c596d98e8b490d06ca763be1a88849e780ddcc74`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 1.3 MB (1264435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad00fa157eebdd61affab09a5b4d3ba310bf443dca82d624ae508b390df30ea6`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:fe5e31b0b4e73341e2002706c4b0fc665dc25f118fee2497eeb4c213283a94c4
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
$ docker pull caddy@sha256:a9cf52bbabc8864aa2bb39cc3b30034060f8b5cfea57a24af5d59fb712a2363d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119514478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972e1302f4350651067d073928bc15bcd5b0219ea111332de1bb9a3eb2af6800`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:14:43 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:14:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:14:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:18:53 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 20:20:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:20:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:20:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:20:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:20:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbbf235a55c104bafc6765f3c92a36489a596041551360d566152f2af01b59`  
		Last Modified: Wed, 31 Mar 2021 20:22:25 GMT  
		Size: 280.9 KB (280881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f184a059628efa0b05f924f5b1e223377ebd57cdec0597912aabcd4b2129b`  
		Last Modified: Wed, 31 Mar 2021 20:23:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec81731eed009f8d947489208d3bc2fe161411bd6ad9543fc2af27bb229d352`  
		Last Modified: Wed, 31 Mar 2021 20:26:05 GMT  
		Size: 106.8 MB (106811699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec2af768a6dad08fb2f9bf5396591d7ab1b7bff816d42c96f7c5169ab05502`  
		Last Modified: Wed, 31 Mar 2021 20:25:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d41b37a714ddeeea16e8fb5e39787ea218dc37873bcc66c101e72177214f54`  
		Last Modified: Thu, 01 Apr 2021 13:54:35 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30dccfb57aae7671a60a9a97a865cdfb7223a51d8d176ca6c833f95a3d0c3`  
		Last Modified: Thu, 01 Apr 2021 13:54:36 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c224dde9c00bfc5be3cc063759e6e39bb2d1586ad856299e4dc5edcbce99ea0d`  
		Last Modified: Thu, 01 Apr 2021 13:54:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:528de32f232e1620d7a832171f2de05db14a38b0367b601508a3554ee39609d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cb88e37729e6535c0e5d37dd52aabf2191db2fc10d3a2d5cc2befb4a3547e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:45:17 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:45:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:45:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:13:42 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 19:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 19:21:40 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 19:21:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 19:21:45 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:04:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:00 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:02 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 04:05:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa6796eed51884cd0436f134281af9489342ecf256aec0b31ca83f254ccd0d1`  
		Last Modified: Wed, 31 Mar 2021 19:23:16 GMT  
		Size: 281.0 KB (280979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c043dc86373f816c29db582d9bddada9a00eeb3812a357a2dfd8e3f68d9a413`  
		Last Modified: Wed, 31 Mar 2021 19:23:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031875ceeaab9b0b96a47b7ed9ec2a0098a9d8662d1c2a57785eb95dbf36d419`  
		Last Modified: Wed, 31 Mar 2021 19:25:23 GMT  
		Size: 102.7 MB (102671786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15870044ac3cd6474d13a6fd94871020ad8801d56fa4387bb9507968da9b093d`  
		Last Modified: Wed, 31 Mar 2021 19:24:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa970c15af3c0912614e0bd697d3329aa1d7f2e98e13f86227bec493367295`  
		Last Modified: Thu, 01 Apr 2021 04:06:04 GMT  
		Size: 7.9 MB (7929419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231389672c1c8c7a9fd39092006eca8983b058e9edc5f0d04bf43bc3f9dea700`  
		Last Modified: Thu, 01 Apr 2021 04:06:02 GMT  
		Size: 1.2 MB (1221595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efaab869ceebc633c179dc051159fb587f7bb30890e765be3f630558cc9933c`  
		Last Modified: Thu, 01 Apr 2021 04:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:673ccce087f4fef545f63f971a0738dbb551fa5872c1742be37a89daded09f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83363f4d6122099578251753b8d8052a348737a2593393b43b431795fcb64292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:56:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:56:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:56:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:36:58 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 01 Apr 2021 12:59:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 12:59:20 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 12:59:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:59:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 12:59:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:27 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 14:30:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:30:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b725919da0175e4c01c41441c29fff6f5ec6c0c4e37417f70120f08f96acfc`  
		Last Modified: Thu, 01 Apr 2021 13:01:16 GMT  
		Size: 280.1 KB (280073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1f51d8714e34d5e746102b7176e77e8142ecf71f4c68d82354285a0bd6d16`  
		Last Modified: Thu, 01 Apr 2021 13:01:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9a84aba5c985724e2f9d0049434534ed654c74b46945f50cc2af08567b9b6`  
		Last Modified: Thu, 01 Apr 2021 13:03:20 GMT  
		Size: 102.5 MB (102462580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc655d7de77ca2ce887998caba1ec52a0bd3f8aa5453bb583ba83449613e96c5`  
		Last Modified: Thu, 01 Apr 2021 13:02:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c177cdf044a6b683b9c1a95121917806970172353334871227cb79e618bc0b1`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1d6a25abce1b9f81c345e1c2ac0149a173ffdcdca04c5ffd9a450903aa2d2`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 1.2 MB (1219450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1bc2f6f317df593b6011ce90f58a1234127d7f78cf8121f8972f79d564b69`  
		Last Modified: Thu, 01 Apr 2021 14:31:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e8c8a0956ea40a17133ef7055aa4cd1076f944342cddf3665d91c8addbe8effb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8892c660131d71ee38d69f56f72c5e98aed80471af824bd1ceda7b5a08c2ce4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:51:33 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:57:28 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:00:54 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:01:02 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:11:38 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 16:11:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:11:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:11:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:11:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f941853f4c183d3b0a653353ba7515088ae2488b01a0ca6bddaa6f1dcc062d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 281.2 KB (281215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4be3bf1d235e013412b55ba1e824da6cfebaf80d284481002d2aa00718563d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc4f0c823675028e8e8caed39be27c63850615a4394ab508faf5b4ed3a9fc3`  
		Last Modified: Fri, 26 Mar 2021 01:04:37 GMT  
		Size: 102.1 MB (102143643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ce0d84f3cb43a1eb06c18a87965b988275ab2c863043b96032d5d4b94d5db`  
		Last Modified: Fri, 26 Mar 2021 01:04:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6274beb5e6ef4051612c2bcfadde952a3caceb7145e9f6d61ce0b818f2e4f7`  
		Last Modified: Fri, 26 Mar 2021 16:12:33 GMT  
		Size: 8.5 MB (8500012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880cf9840fe472a748b59dbd60483c321b780ac76a1906aafe3c082bfd41496d`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 1.2 MB (1201557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d154a0032206067bed60392933ce1a8bab8e7cd48226b92f0f589d7f1bd746`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b84ae4910f796380e57d7daac89af75d8012094746a88fa467d97bafcdb11fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113985368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b7945ba534d20ab228061857652036740c946d79102221e87b9fb0ea979254`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:50:54 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:58:55 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:01:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:01:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:01:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:02:00 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:52:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:52:17 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:52:23 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:52:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:52:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:52:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22fc023a51f1560551f97595c0d26436968276b81fd2119cb972238aff23fb6`  
		Last Modified: Fri, 26 Mar 2021 01:06:49 GMT  
		Size: 283.2 KB (283209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b5b049d7abfca6a07577171113a612a55eb6f864651563d204b02fb5c4e60`  
		Last Modified: Fri, 26 Mar 2021 01:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db853427f2ec5049b1f9079b25be4c8117deaa1fcac132410fa8c0b1deb720c8`  
		Last Modified: Fri, 26 Mar 2021 01:12:48 GMT  
		Size: 100.8 MB (100803535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d927b70afd72e9dd133e5d57a45143c8e8ebceefa2dfc3a7fc1bd8e1b9ce83d8`  
		Last Modified: Fri, 26 Mar 2021 01:12:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf5bc1fa9c61f972e646bacb633a53efd7d173b4d79b2efd32f923d503d50b`  
		Last Modified: Fri, 26 Mar 2021 05:58:21 GMT  
		Size: 8.9 MB (8921440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6874c8aee6bfafc6a12719998f12ce1dcf70d8a61da3dd914f9c791808221`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0826f628855fe686aafb0d3423a1c5258fcb72287998561865187f7e7d4f0`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e7648a8c6fc41f80b2eb8da973742a7485f479cb4f57dcb04d738e8800f5b64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118389839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8b0338c771c7f370f6460e6a444505905acc419685f5c8d35648800e50d8c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:34:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:34:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:34:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:38:18 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 18:39:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:39:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:39:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:39:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:39:47 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:15 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb296d6fc71cd9057e3d03d0ea4ebe30a620f7c6ce57eb78f4c137e77a9a47`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 281.4 KB (281355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783b7db1c405d51f50a261ae252c97941c44ffeb93cb10c2e2bdd458296774a`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb58064707977215f9632cdb206eaec9d63534f602e5682c22634dcfbb2cbd5`  
		Last Modified: Wed, 31 Mar 2021 18:42:02 GMT  
		Size: 105.9 MB (105923109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273a64a6b34c09c3baa0d7e2dc15a36980a72e658c1570903625ebac61f7f16`  
		Last Modified: Wed, 31 Mar 2021 18:41:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadae105e5bbdd611f262c9d81668d5b3251f7c246bd9bd444ecd4c88b936326`  
		Last Modified: Wed, 31 Mar 2021 18:57:12 GMT  
		Size: 8.4 MB (8352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7739fc64956105cdc380f5c596d98e8b490d06ca763be1a88849e780ddcc74`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 1.3 MB (1264435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad00fa157eebdd61affab09a5b4d3ba310bf443dca82d624ae508b390df30ea6`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:abf97331ba731afdbe77aafef9738f37f5073739ad99cdced920c974c73ca4f4
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
$ docker pull caddy@sha256:629c5800ccf51df482a4e63266e4570de3e573e862d902398b03cbfca2212b4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e073d63a624f18bd8e2f94b9e84715e5a33a817db19afa42afc8ea95e59d568`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:17 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:24 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc82ca1670c70e5b605729b271409acba02ca26c3f669bf1d95a067fb853a90`  
		Last Modified: Thu, 01 Apr 2021 13:54:20 GMT  
		Size: 300.0 KB (300021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d66f69260e9358ba74c27e0ed110b9ff7781c5f90d5d01f86d6ef289834382`  
		Last Modified: Thu, 01 Apr 2021 13:54:17 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b38557b1fd80a7712b7263f0896f076afdeb9f25f68a79e288b87490aa3047`  
		Last Modified: Thu, 01 Apr 2021 13:54:19 GMT  
		Size: 11.6 MB (11622380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37d6fba45d5f1633f00b6a9d204abacad2a6918dc355706fe0decc0bc4e565`  
		Last Modified: Thu, 01 Apr 2021 13:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b57cdc61b54865a7ff2ea4ef9d16458537d40e0dc25559d6540111874abbe4ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88293e19906b6b2275ff6e127e29960b1fdf0cf0c4baa4bbce4ea297e90db731`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:36:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:36:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:36:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 17:36:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:36:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:36:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:36:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:36:56 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 17:36:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:36:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:37:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:37:07 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:37:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:37:10 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:37:11 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:37:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1532456df32c320ccd3c9ff5433c9e44d873ef87a0dc9fc29f9cf256b517eb4`  
		Last Modified: Wed, 31 Mar 2021 17:38:50 GMT  
		Size: 300.1 KB (300103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263f61714ef61a0c59bef8e70bc49a741a357b0a0fc556b44f8344df37ea0f8`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818002dab28746359de43d5a88d06c77cc3a353c838e15c6b6a67d48352cc5c0`  
		Last Modified: Wed, 31 Mar 2021 17:38:54 GMT  
		Size: 10.9 MB (10944835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979a3c808bf5c07c668f5966a15458dbfe9aba5aa7d761e690dd3a5cadf45eb`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6d510324512c20fc0d40aeb8b6e5b98255c857ad2dee894b6cb6e66f0231cf9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42db38da968682707e6cf0fabb16f93770388907d8a208fca0db74cae3183ba2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:11:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:11:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:11:48 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 08:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:11:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:11:56 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:11:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:11:58 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:11:59 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 08:12:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:12:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:12:09 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:12:11 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:12:13 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:12:15 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:12:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547b5d01ba24abc02b4f05f8134bfb156ce1840f496ed03a1316c882625bd41f`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 299.2 KB (299199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a883a914d37801ae97b0fac82c62e4f70ef4c92fc53417a91a23b2e69d36d9bb`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475143e7b89d1a36700916ec3c8f0caae9b57d5cd9ba187b9f3fd5d9a71eddcf`  
		Last Modified: Thu, 01 Apr 2021 08:13:38 GMT  
		Size: 10.9 MB (10925346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79cdab22a3397c4a98f63a7e96c51881033744b1f198c4984072e7303e9f73`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1c3e6c1b947162789190f9215b56c517caa5c48bd5d09f9753c6ff105ece8ea4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d36a254c95d4ad655ca159d67b79ad8ca4498f82a3c127340a7b5be09e213b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:40:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:40:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:40:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 12:40:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:40:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:40:35 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:40:38 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:40:44 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:40:49 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:40:53 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 12:40:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:40:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:40:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:40:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:40:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:41:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:41:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:41:05 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:41:08 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:41:12 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:41:18 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1fbebcb85e1b4f7457195688308678e46184f78ec8402dcd4eb0992700541`  
		Last Modified: Thu, 01 Apr 2021 12:45:24 GMT  
		Size: 300.3 KB (300333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c34c85964e1be21b929d726522dfd448c029aaf7acd32bf5342ff93070124bd`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c657d5761128c010be222b8ddea92ceba700a3c76afb7704c9d436bbb5582c1`  
		Last Modified: Thu, 01 Apr 2021 12:45:27 GMT  
		Size: 10.6 MB (10598978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90c89f24747de4d19b1c83875e0072662bfe7ce4c5f4e15c551d907b212ebc`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:d8ff14acdf013e9a2df27d95f3326bf7175307a04e9e6f7a40b840bf813898ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63b8a5e4185f59e46edc1e47b15d592327b0c3b8867d3edd3be3a9b3dea5522`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:49:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:49:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:49:51 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:50:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:50:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:50:24 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:50:30 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:50:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 05:50:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:50:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:50:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:50:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:50:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:51:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:51:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:51:24 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:51:30 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:51:35 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:51:40 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:51:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69ab62cc22d6fb5ba7a45731c0b8f378026c7c711d7d48946bfe7c69eae199`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 302.3 KB (302337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9767f7d2aec64fa7c89aa12c9b2b14b03dbe10e20cf53279a88f5009dd2c7841`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502018de7a2dcf0f08830ebcce7c073c9a9db95ecf366d96d44c7a76ba032edc`  
		Last Modified: Fri, 26 Mar 2021 05:58:02 GMT  
		Size: 10.2 MB (10241383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61815e7304b64383c90b6c68c7220f40b74c932f3dd3cfd44b04fed05920aec`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; s390x

```console
$ docker pull caddy@sha256:9d992badb7530225182676af12ae945f5f2de2f5ad7d3946b397892a6de4c123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c8a68869d0806c29e6c2c9c655d3e9085af285c6c24ea651ad3bdffd714e38`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:55:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:00 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:05 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:06 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:08 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8eb19b6319d0b09121581759094c3eb58e5574e2063affb6c42c0e1a1937a0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd6e269a873b8a21e2787b0ea05662c0f2676aa9043f52b8884081965be7112`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f6a8a7e19cb11edbda771ce361181202915f4760cdaef5e290b1758cc7b88c`  
		Last Modified: Wed, 31 Mar 2021 18:57:02 GMT  
		Size: 11.3 MB (11272066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec92d2dcab4ee41e4e626d8b360a6feff3822db894894865a36bbe9cfc759df0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:a18e9c84fb32bae7eeaab4b048f10c4ec8797e4641f8d7d5f75d35e11282d0e3
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
$ docker pull caddy@sha256:629c5800ccf51df482a4e63266e4570de3e573e862d902398b03cbfca2212b4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e073d63a624f18bd8e2f94b9e84715e5a33a817db19afa42afc8ea95e59d568`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:17 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:24 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc82ca1670c70e5b605729b271409acba02ca26c3f669bf1d95a067fb853a90`  
		Last Modified: Thu, 01 Apr 2021 13:54:20 GMT  
		Size: 300.0 KB (300021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d66f69260e9358ba74c27e0ed110b9ff7781c5f90d5d01f86d6ef289834382`  
		Last Modified: Thu, 01 Apr 2021 13:54:17 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b38557b1fd80a7712b7263f0896f076afdeb9f25f68a79e288b87490aa3047`  
		Last Modified: Thu, 01 Apr 2021 13:54:19 GMT  
		Size: 11.6 MB (11622380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37d6fba45d5f1633f00b6a9d204abacad2a6918dc355706fe0decc0bc4e565`  
		Last Modified: Thu, 01 Apr 2021 13:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b57cdc61b54865a7ff2ea4ef9d16458537d40e0dc25559d6540111874abbe4ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88293e19906b6b2275ff6e127e29960b1fdf0cf0c4baa4bbce4ea297e90db731`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:36:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:36:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:36:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 17:36:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:36:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:36:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:36:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:36:56 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 17:36:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:36:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:37:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:37:07 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:37:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:37:10 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:37:11 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:37:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1532456df32c320ccd3c9ff5433c9e44d873ef87a0dc9fc29f9cf256b517eb4`  
		Last Modified: Wed, 31 Mar 2021 17:38:50 GMT  
		Size: 300.1 KB (300103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263f61714ef61a0c59bef8e70bc49a741a357b0a0fc556b44f8344df37ea0f8`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818002dab28746359de43d5a88d06c77cc3a353c838e15c6b6a67d48352cc5c0`  
		Last Modified: Wed, 31 Mar 2021 17:38:54 GMT  
		Size: 10.9 MB (10944835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979a3c808bf5c07c668f5966a15458dbfe9aba5aa7d761e690dd3a5cadf45eb`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6d510324512c20fc0d40aeb8b6e5b98255c857ad2dee894b6cb6e66f0231cf9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42db38da968682707e6cf0fabb16f93770388907d8a208fca0db74cae3183ba2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:11:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:11:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:11:48 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 08:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:11:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:11:56 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:11:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:11:58 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:11:59 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 08:12:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:12:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:12:09 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:12:11 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:12:13 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:12:15 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:12:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547b5d01ba24abc02b4f05f8134bfb156ce1840f496ed03a1316c882625bd41f`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 299.2 KB (299199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a883a914d37801ae97b0fac82c62e4f70ef4c92fc53417a91a23b2e69d36d9bb`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475143e7b89d1a36700916ec3c8f0caae9b57d5cd9ba187b9f3fd5d9a71eddcf`  
		Last Modified: Thu, 01 Apr 2021 08:13:38 GMT  
		Size: 10.9 MB (10925346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79cdab22a3397c4a98f63a7e96c51881033744b1f198c4984072e7303e9f73`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1c3e6c1b947162789190f9215b56c517caa5c48bd5d09f9753c6ff105ece8ea4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d36a254c95d4ad655ca159d67b79ad8ca4498f82a3c127340a7b5be09e213b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:40:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:40:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:40:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 12:40:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:40:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:40:35 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:40:38 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:40:44 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:40:49 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:40:53 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 12:40:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:40:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:40:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:40:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:40:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:41:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:41:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:41:05 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:41:08 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:41:12 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:41:18 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1fbebcb85e1b4f7457195688308678e46184f78ec8402dcd4eb0992700541`  
		Last Modified: Thu, 01 Apr 2021 12:45:24 GMT  
		Size: 300.3 KB (300333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c34c85964e1be21b929d726522dfd448c029aaf7acd32bf5342ff93070124bd`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c657d5761128c010be222b8ddea92ceba700a3c76afb7704c9d436bbb5582c1`  
		Last Modified: Thu, 01 Apr 2021 12:45:27 GMT  
		Size: 10.6 MB (10598978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90c89f24747de4d19b1c83875e0072662bfe7ce4c5f4e15c551d907b212ebc`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d8ff14acdf013e9a2df27d95f3326bf7175307a04e9e6f7a40b840bf813898ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63b8a5e4185f59e46edc1e47b15d592327b0c3b8867d3edd3be3a9b3dea5522`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:49:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:49:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:49:51 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:50:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:50:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:50:24 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:50:30 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:50:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 05:50:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:50:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:50:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:50:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:50:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:51:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:51:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:51:24 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:51:30 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:51:35 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:51:40 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:51:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69ab62cc22d6fb5ba7a45731c0b8f378026c7c711d7d48946bfe7c69eae199`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 302.3 KB (302337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9767f7d2aec64fa7c89aa12c9b2b14b03dbe10e20cf53279a88f5009dd2c7841`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502018de7a2dcf0f08830ebcce7c073c9a9db95ecf366d96d44c7a76ba032edc`  
		Last Modified: Fri, 26 Mar 2021 05:58:02 GMT  
		Size: 10.2 MB (10241383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61815e7304b64383c90b6c68c7220f40b74c932f3dd3cfd44b04fed05920aec`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9d992badb7530225182676af12ae945f5f2de2f5ad7d3946b397892a6de4c123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c8a68869d0806c29e6c2c9c655d3e9085af285c6c24ea651ad3bdffd714e38`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:55:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:00 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:05 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:06 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:08 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8eb19b6319d0b09121581759094c3eb58e5574e2063affb6c42c0e1a1937a0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd6e269a873b8a21e2787b0ea05662c0f2676aa9043f52b8884081965be7112`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f6a8a7e19cb11edbda771ce361181202915f4760cdaef5e290b1758cc7b88c`  
		Last Modified: Wed, 31 Mar 2021 18:57:02 GMT  
		Size: 11.3 MB (11272066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec92d2dcab4ee41e4e626d8b360a6feff3822db894894865a36bbe9cfc759df0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder`

```console
$ docker pull caddy@sha256:803eb2fbf7bc2389c531d241d9596982a84cb74a9d37fc2659e95c3f8ebeccaf
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
$ docker pull caddy@sha256:a9cf52bbabc8864aa2bb39cc3b30034060f8b5cfea57a24af5d59fb712a2363d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119514478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972e1302f4350651067d073928bc15bcd5b0219ea111332de1bb9a3eb2af6800`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:14:43 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:14:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:14:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:18:53 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 20:20:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:20:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:20:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:20:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:20:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbbf235a55c104bafc6765f3c92a36489a596041551360d566152f2af01b59`  
		Last Modified: Wed, 31 Mar 2021 20:22:25 GMT  
		Size: 280.9 KB (280881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f184a059628efa0b05f924f5b1e223377ebd57cdec0597912aabcd4b2129b`  
		Last Modified: Wed, 31 Mar 2021 20:23:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec81731eed009f8d947489208d3bc2fe161411bd6ad9543fc2af27bb229d352`  
		Last Modified: Wed, 31 Mar 2021 20:26:05 GMT  
		Size: 106.8 MB (106811699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec2af768a6dad08fb2f9bf5396591d7ab1b7bff816d42c96f7c5169ab05502`  
		Last Modified: Wed, 31 Mar 2021 20:25:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d41b37a714ddeeea16e8fb5e39787ea218dc37873bcc66c101e72177214f54`  
		Last Modified: Thu, 01 Apr 2021 13:54:35 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30dccfb57aae7671a60a9a97a865cdfb7223a51d8d176ca6c833f95a3d0c3`  
		Last Modified: Thu, 01 Apr 2021 13:54:36 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c224dde9c00bfc5be3cc063759e6e39bb2d1586ad856299e4dc5edcbce99ea0d`  
		Last Modified: Thu, 01 Apr 2021 13:54:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:528de32f232e1620d7a832171f2de05db14a38b0367b601508a3554ee39609d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cb88e37729e6535c0e5d37dd52aabf2191db2fc10d3a2d5cc2befb4a3547e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:45:17 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:45:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:45:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:13:42 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 19:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 19:21:40 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 19:21:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 19:21:45 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:04:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:00 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:02 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 04:05:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa6796eed51884cd0436f134281af9489342ecf256aec0b31ca83f254ccd0d1`  
		Last Modified: Wed, 31 Mar 2021 19:23:16 GMT  
		Size: 281.0 KB (280979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c043dc86373f816c29db582d9bddada9a00eeb3812a357a2dfd8e3f68d9a413`  
		Last Modified: Wed, 31 Mar 2021 19:23:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031875ceeaab9b0b96a47b7ed9ec2a0098a9d8662d1c2a57785eb95dbf36d419`  
		Last Modified: Wed, 31 Mar 2021 19:25:23 GMT  
		Size: 102.7 MB (102671786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15870044ac3cd6474d13a6fd94871020ad8801d56fa4387bb9507968da9b093d`  
		Last Modified: Wed, 31 Mar 2021 19:24:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa970c15af3c0912614e0bd697d3329aa1d7f2e98e13f86227bec493367295`  
		Last Modified: Thu, 01 Apr 2021 04:06:04 GMT  
		Size: 7.9 MB (7929419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231389672c1c8c7a9fd39092006eca8983b058e9edc5f0d04bf43bc3f9dea700`  
		Last Modified: Thu, 01 Apr 2021 04:06:02 GMT  
		Size: 1.2 MB (1221595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efaab869ceebc633c179dc051159fb587f7bb30890e765be3f630558cc9933c`  
		Last Modified: Thu, 01 Apr 2021 04:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:673ccce087f4fef545f63f971a0738dbb551fa5872c1742be37a89daded09f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83363f4d6122099578251753b8d8052a348737a2593393b43b431795fcb64292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:56:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:56:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:56:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:36:58 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 01 Apr 2021 12:59:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 12:59:20 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 12:59:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:59:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 12:59:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:27 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 14:30:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:30:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b725919da0175e4c01c41441c29fff6f5ec6c0c4e37417f70120f08f96acfc`  
		Last Modified: Thu, 01 Apr 2021 13:01:16 GMT  
		Size: 280.1 KB (280073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1f51d8714e34d5e746102b7176e77e8142ecf71f4c68d82354285a0bd6d16`  
		Last Modified: Thu, 01 Apr 2021 13:01:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9a84aba5c985724e2f9d0049434534ed654c74b46945f50cc2af08567b9b6`  
		Last Modified: Thu, 01 Apr 2021 13:03:20 GMT  
		Size: 102.5 MB (102462580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc655d7de77ca2ce887998caba1ec52a0bd3f8aa5453bb583ba83449613e96c5`  
		Last Modified: Thu, 01 Apr 2021 13:02:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c177cdf044a6b683b9c1a95121917806970172353334871227cb79e618bc0b1`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1d6a25abce1b9f81c345e1c2ac0149a173ffdcdca04c5ffd9a450903aa2d2`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 1.2 MB (1219450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1bc2f6f317df593b6011ce90f58a1234127d7f78cf8121f8972f79d564b69`  
		Last Modified: Thu, 01 Apr 2021 14:31:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e8c8a0956ea40a17133ef7055aa4cd1076f944342cddf3665d91c8addbe8effb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8892c660131d71ee38d69f56f72c5e98aed80471af824bd1ceda7b5a08c2ce4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:51:33 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:57:28 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:00:54 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:01:02 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:11:38 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 16:11:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:11:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:11:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:11:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f941853f4c183d3b0a653353ba7515088ae2488b01a0ca6bddaa6f1dcc062d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 281.2 KB (281215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4be3bf1d235e013412b55ba1e824da6cfebaf80d284481002d2aa00718563d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc4f0c823675028e8e8caed39be27c63850615a4394ab508faf5b4ed3a9fc3`  
		Last Modified: Fri, 26 Mar 2021 01:04:37 GMT  
		Size: 102.1 MB (102143643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ce0d84f3cb43a1eb06c18a87965b988275ab2c863043b96032d5d4b94d5db`  
		Last Modified: Fri, 26 Mar 2021 01:04:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6274beb5e6ef4051612c2bcfadde952a3caceb7145e9f6d61ce0b818f2e4f7`  
		Last Modified: Fri, 26 Mar 2021 16:12:33 GMT  
		Size: 8.5 MB (8500012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880cf9840fe472a748b59dbd60483c321b780ac76a1906aafe3c082bfd41496d`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 1.2 MB (1201557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d154a0032206067bed60392933ce1a8bab8e7cd48226b92f0f589d7f1bd746`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:b84ae4910f796380e57d7daac89af75d8012094746a88fa467d97bafcdb11fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113985368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b7945ba534d20ab228061857652036740c946d79102221e87b9fb0ea979254`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:50:54 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:58:55 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:01:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:01:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:01:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:02:00 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:52:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:52:17 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:52:23 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:52:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:52:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:52:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22fc023a51f1560551f97595c0d26436968276b81fd2119cb972238aff23fb6`  
		Last Modified: Fri, 26 Mar 2021 01:06:49 GMT  
		Size: 283.2 KB (283209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b5b049d7abfca6a07577171113a612a55eb6f864651563d204b02fb5c4e60`  
		Last Modified: Fri, 26 Mar 2021 01:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db853427f2ec5049b1f9079b25be4c8117deaa1fcac132410fa8c0b1deb720c8`  
		Last Modified: Fri, 26 Mar 2021 01:12:48 GMT  
		Size: 100.8 MB (100803535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d927b70afd72e9dd133e5d57a45143c8e8ebceefa2dfc3a7fc1bd8e1b9ce83d8`  
		Last Modified: Fri, 26 Mar 2021 01:12:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf5bc1fa9c61f972e646bacb633a53efd7d173b4d79b2efd32f923d503d50b`  
		Last Modified: Fri, 26 Mar 2021 05:58:21 GMT  
		Size: 8.9 MB (8921440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6874c8aee6bfafc6a12719998f12ce1dcf70d8a61da3dd914f9c791808221`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0826f628855fe686aafb0d3423a1c5258fcb72287998561865187f7e7d4f0`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:e7648a8c6fc41f80b2eb8da973742a7485f479cb4f57dcb04d738e8800f5b64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118389839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8b0338c771c7f370f6460e6a444505905acc419685f5c8d35648800e50d8c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:34:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:34:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:34:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:38:18 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 18:39:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:39:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:39:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:39:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:39:47 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:15 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb296d6fc71cd9057e3d03d0ea4ebe30a620f7c6ce57eb78f4c137e77a9a47`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 281.4 KB (281355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783b7db1c405d51f50a261ae252c97941c44ffeb93cb10c2e2bdd458296774a`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb58064707977215f9632cdb206eaec9d63534f602e5682c22634dcfbb2cbd5`  
		Last Modified: Wed, 31 Mar 2021 18:42:02 GMT  
		Size: 105.9 MB (105923109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273a64a6b34c09c3baa0d7e2dc15a36980a72e658c1570903625ebac61f7f16`  
		Last Modified: Wed, 31 Mar 2021 18:41:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadae105e5bbdd611f262c9d81668d5b3251f7c246bd9bd444ecd4c88b936326`  
		Last Modified: Wed, 31 Mar 2021 18:57:12 GMT  
		Size: 8.4 MB (8352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7739fc64956105cdc380f5c596d98e8b490d06ca763be1a88849e780ddcc74`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 1.3 MB (1264435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad00fa157eebdd61affab09a5b4d3ba310bf443dca82d624ae508b390df30ea6`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:fe5e31b0b4e73341e2002706c4b0fc665dc25f118fee2497eeb4c213283a94c4
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
$ docker pull caddy@sha256:a9cf52bbabc8864aa2bb39cc3b30034060f8b5cfea57a24af5d59fb712a2363d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119514478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972e1302f4350651067d073928bc15bcd5b0219ea111332de1bb9a3eb2af6800`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:14:43 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:14:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:14:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:18:53 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 20:20:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:20:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:20:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:20:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:20:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbbf235a55c104bafc6765f3c92a36489a596041551360d566152f2af01b59`  
		Last Modified: Wed, 31 Mar 2021 20:22:25 GMT  
		Size: 280.9 KB (280881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f184a059628efa0b05f924f5b1e223377ebd57cdec0597912aabcd4b2129b`  
		Last Modified: Wed, 31 Mar 2021 20:23:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec81731eed009f8d947489208d3bc2fe161411bd6ad9543fc2af27bb229d352`  
		Last Modified: Wed, 31 Mar 2021 20:26:05 GMT  
		Size: 106.8 MB (106811699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec2af768a6dad08fb2f9bf5396591d7ab1b7bff816d42c96f7c5169ab05502`  
		Last Modified: Wed, 31 Mar 2021 20:25:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d41b37a714ddeeea16e8fb5e39787ea218dc37873bcc66c101e72177214f54`  
		Last Modified: Thu, 01 Apr 2021 13:54:35 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30dccfb57aae7671a60a9a97a865cdfb7223a51d8d176ca6c833f95a3d0c3`  
		Last Modified: Thu, 01 Apr 2021 13:54:36 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c224dde9c00bfc5be3cc063759e6e39bb2d1586ad856299e4dc5edcbce99ea0d`  
		Last Modified: Thu, 01 Apr 2021 13:54:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:528de32f232e1620d7a832171f2de05db14a38b0367b601508a3554ee39609d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cb88e37729e6535c0e5d37dd52aabf2191db2fc10d3a2d5cc2befb4a3547e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:45:17 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:45:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:45:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:13:42 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 19:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 19:21:40 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 19:21:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 19:21:45 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:04:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:00 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:02 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 04:05:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa6796eed51884cd0436f134281af9489342ecf256aec0b31ca83f254ccd0d1`  
		Last Modified: Wed, 31 Mar 2021 19:23:16 GMT  
		Size: 281.0 KB (280979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c043dc86373f816c29db582d9bddada9a00eeb3812a357a2dfd8e3f68d9a413`  
		Last Modified: Wed, 31 Mar 2021 19:23:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031875ceeaab9b0b96a47b7ed9ec2a0098a9d8662d1c2a57785eb95dbf36d419`  
		Last Modified: Wed, 31 Mar 2021 19:25:23 GMT  
		Size: 102.7 MB (102671786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15870044ac3cd6474d13a6fd94871020ad8801d56fa4387bb9507968da9b093d`  
		Last Modified: Wed, 31 Mar 2021 19:24:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa970c15af3c0912614e0bd697d3329aa1d7f2e98e13f86227bec493367295`  
		Last Modified: Thu, 01 Apr 2021 04:06:04 GMT  
		Size: 7.9 MB (7929419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231389672c1c8c7a9fd39092006eca8983b058e9edc5f0d04bf43bc3f9dea700`  
		Last Modified: Thu, 01 Apr 2021 04:06:02 GMT  
		Size: 1.2 MB (1221595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efaab869ceebc633c179dc051159fb587f7bb30890e765be3f630558cc9933c`  
		Last Modified: Thu, 01 Apr 2021 04:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:673ccce087f4fef545f63f971a0738dbb551fa5872c1742be37a89daded09f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83363f4d6122099578251753b8d8052a348737a2593393b43b431795fcb64292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:56:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:56:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:56:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:36:58 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 01 Apr 2021 12:59:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 12:59:20 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 12:59:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:59:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 12:59:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:27 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 14:30:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:30:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b725919da0175e4c01c41441c29fff6f5ec6c0c4e37417f70120f08f96acfc`  
		Last Modified: Thu, 01 Apr 2021 13:01:16 GMT  
		Size: 280.1 KB (280073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1f51d8714e34d5e746102b7176e77e8142ecf71f4c68d82354285a0bd6d16`  
		Last Modified: Thu, 01 Apr 2021 13:01:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9a84aba5c985724e2f9d0049434534ed654c74b46945f50cc2af08567b9b6`  
		Last Modified: Thu, 01 Apr 2021 13:03:20 GMT  
		Size: 102.5 MB (102462580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc655d7de77ca2ce887998caba1ec52a0bd3f8aa5453bb583ba83449613e96c5`  
		Last Modified: Thu, 01 Apr 2021 13:02:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c177cdf044a6b683b9c1a95121917806970172353334871227cb79e618bc0b1`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1d6a25abce1b9f81c345e1c2ac0149a173ffdcdca04c5ffd9a450903aa2d2`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 1.2 MB (1219450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1bc2f6f317df593b6011ce90f58a1234127d7f78cf8121f8972f79d564b69`  
		Last Modified: Thu, 01 Apr 2021 14:31:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e8c8a0956ea40a17133ef7055aa4cd1076f944342cddf3665d91c8addbe8effb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8892c660131d71ee38d69f56f72c5e98aed80471af824bd1ceda7b5a08c2ce4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:51:33 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:57:28 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:00:54 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:01:02 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:11:38 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 16:11:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:11:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:11:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:11:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f941853f4c183d3b0a653353ba7515088ae2488b01a0ca6bddaa6f1dcc062d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 281.2 KB (281215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4be3bf1d235e013412b55ba1e824da6cfebaf80d284481002d2aa00718563d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc4f0c823675028e8e8caed39be27c63850615a4394ab508faf5b4ed3a9fc3`  
		Last Modified: Fri, 26 Mar 2021 01:04:37 GMT  
		Size: 102.1 MB (102143643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ce0d84f3cb43a1eb06c18a87965b988275ab2c863043b96032d5d4b94d5db`  
		Last Modified: Fri, 26 Mar 2021 01:04:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6274beb5e6ef4051612c2bcfadde952a3caceb7145e9f6d61ce0b818f2e4f7`  
		Last Modified: Fri, 26 Mar 2021 16:12:33 GMT  
		Size: 8.5 MB (8500012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880cf9840fe472a748b59dbd60483c321b780ac76a1906aafe3c082bfd41496d`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 1.2 MB (1201557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d154a0032206067bed60392933ce1a8bab8e7cd48226b92f0f589d7f1bd746`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b84ae4910f796380e57d7daac89af75d8012094746a88fa467d97bafcdb11fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113985368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b7945ba534d20ab228061857652036740c946d79102221e87b9fb0ea979254`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:50:54 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:58:55 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:01:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:01:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:01:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:02:00 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:52:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:52:17 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:52:23 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:52:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:52:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:52:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22fc023a51f1560551f97595c0d26436968276b81fd2119cb972238aff23fb6`  
		Last Modified: Fri, 26 Mar 2021 01:06:49 GMT  
		Size: 283.2 KB (283209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b5b049d7abfca6a07577171113a612a55eb6f864651563d204b02fb5c4e60`  
		Last Modified: Fri, 26 Mar 2021 01:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db853427f2ec5049b1f9079b25be4c8117deaa1fcac132410fa8c0b1deb720c8`  
		Last Modified: Fri, 26 Mar 2021 01:12:48 GMT  
		Size: 100.8 MB (100803535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d927b70afd72e9dd133e5d57a45143c8e8ebceefa2dfc3a7fc1bd8e1b9ce83d8`  
		Last Modified: Fri, 26 Mar 2021 01:12:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf5bc1fa9c61f972e646bacb633a53efd7d173b4d79b2efd32f923d503d50b`  
		Last Modified: Fri, 26 Mar 2021 05:58:21 GMT  
		Size: 8.9 MB (8921440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6874c8aee6bfafc6a12719998f12ce1dcf70d8a61da3dd914f9c791808221`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0826f628855fe686aafb0d3423a1c5258fcb72287998561865187f7e7d4f0`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e7648a8c6fc41f80b2eb8da973742a7485f479cb4f57dcb04d738e8800f5b64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118389839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8b0338c771c7f370f6460e6a444505905acc419685f5c8d35648800e50d8c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:34:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:34:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:34:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:38:18 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 18:39:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:39:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:39:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:39:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:39:47 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:15 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb296d6fc71cd9057e3d03d0ea4ebe30a620f7c6ce57eb78f4c137e77a9a47`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 281.4 KB (281355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783b7db1c405d51f50a261ae252c97941c44ffeb93cb10c2e2bdd458296774a`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb58064707977215f9632cdb206eaec9d63534f602e5682c22634dcfbb2cbd5`  
		Last Modified: Wed, 31 Mar 2021 18:42:02 GMT  
		Size: 105.9 MB (105923109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273a64a6b34c09c3baa0d7e2dc15a36980a72e658c1570903625ebac61f7f16`  
		Last Modified: Wed, 31 Mar 2021 18:41:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadae105e5bbdd611f262c9d81668d5b3251f7c246bd9bd444ecd4c88b936326`  
		Last Modified: Wed, 31 Mar 2021 18:57:12 GMT  
		Size: 8.4 MB (8352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7739fc64956105cdc380f5c596d98e8b490d06ca763be1a88849e780ddcc74`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 1.3 MB (1264435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad00fa157eebdd61affab09a5b4d3ba310bf443dca82d624ae508b390df30ea6`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:e6ed0c57db5b662146f196035584eb49eed8ccad9bdf1aaef32c2d08acfdcae9
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
$ docker pull caddy@sha256:90739a174e62e7c2624f9e13c300ae1a0bbd4dd22f65e7bf3738728fc5012355
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14764220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f0db44e95dc004926717fbe5536ff6c84a8b33cb1299f3207a828f6555ba94`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:38 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 13:53:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:42 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:43 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:44 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:45 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:45 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:45 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bb2b56f5f929e2a4dc7d7325b813da8143e5c9e04e10b31c96062a1c6b6dc7`  
		Last Modified: Thu, 01 Apr 2021 13:54:51 GMT  
		Size: 300.4 KB (300410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75d86528dfa0dc68505576f5dca881ac6ec4e2d2d1f722996e4e159c3ef9f12`  
		Last Modified: Thu, 01 Apr 2021 13:54:51 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f54fdea6e3e9cd7e7514b5b7238444c24373003c0eef8b9b8d73463beb7b62f`  
		Last Modified: Thu, 01 Apr 2021 13:54:53 GMT  
		Size: 11.6 MB (11645882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9224309aa0e7a8ae91bfe2da3056b90632f201d22edfa10c6a68ad0749e165e2`  
		Last Modified: Thu, 01 Apr 2021 13:54:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:1c800d34613af552185bb83c9cc5a9a0cd38787f451c4b83711bbd674244aaea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13898546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098705766700a2865c6e2f7a2d17084e261ac1a2f0da1d1f6c1ccbdcc20c2a03`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:37:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:37:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:37:39 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 31 Mar 2021 17:37:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:37:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:37:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:37:50 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:37:51 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:37:52 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:37:53 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 31 Mar 2021 17:37:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:37:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:38:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:38:02 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:38:03 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:38:05 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:38:14 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:38:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c9efa35742ee0a666b515a98db003c485ba9d25f69cf233de1eb63aa39c5c2`  
		Last Modified: Wed, 31 Mar 2021 17:39:06 GMT  
		Size: 300.5 KB (300517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48e60f29a99505017e416055581b9862de29e7cfe6f26070558fb74390f324e`  
		Last Modified: Wed, 31 Mar 2021 17:39:08 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c996908a645bfe2c9cab1f64d06edbfeb540343c809ccbe9a6b402b1bba28024`  
		Last Modified: Wed, 31 Mar 2021 17:39:09 GMT  
		Size: 11.0 MB (10969936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8931aa62a8cba14c6dfee3aba3b7afce08b5811240c3912a1afa5319d20a42`  
		Last Modified: Wed, 31 Mar 2021 17:39:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:eaa63043acac3ff263376e0c4457d3dc81985775df976dbbd787853761bc7005
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13677725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595bb074d36d2f00bfd21d533c746c82f4a87ef97ccd29121533b0eed798df19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:12:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:12:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:12:39 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 08:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:12:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:12:48 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:12:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:12:51 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:12:52 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:53 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Thu, 01 Apr 2021 08:12:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:13:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:13:01 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:13:02 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:13:03 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:13:04 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:13:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005f2c85bbb34689fa5969c0cda8fda42d2b7848e654ff9efd67e02219a40b8f`  
		Last Modified: Thu, 01 Apr 2021 08:13:51 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d7c4a454e535a084cd7750c2ffd66ce60425166f563b6a8ac7f90dee1a6759`  
		Last Modified: Thu, 01 Apr 2021 08:13:51 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50d0ae8db26661487a79db1382dae8decc375f8add033f2e36ee304ba598f56`  
		Last Modified: Thu, 01 Apr 2021 08:13:52 GMT  
		Size: 10.9 MB (10947975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e50d54f6601d35e1dc2b6d4de04c28a5eff573b9524542e0497948c48dfeca`  
		Last Modified: Thu, 01 Apr 2021 08:13:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b6b4390de836d61962839093fb1d5d5979dae94e952eadf29fc3b54c14bcf73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13643504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ffba442e6b59579406ed8336ba2063bcb190ec8d18ab1532ca1aa675b92715`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:42:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:42:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:42:58 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 12:43:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:43:44 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:43:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:43:50 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:43:52 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:43:54 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Thu, 01 Apr 2021 12:43:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:44:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:44:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:44:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:44:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:44:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:44:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:44:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:44:26 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:44:30 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:44:38 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:44:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08584473c2f3ce7502fc1abe444e6fa79a7cc73e3e8d17f7a9907f9dc549309c`  
		Last Modified: Thu, 01 Apr 2021 12:45:41 GMT  
		Size: 300.6 KB (300621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5107f9070ac9919ca292fcdd94a304ba2a137964d1ff68207424289ef928f`  
		Last Modified: Thu, 01 Apr 2021 12:45:41 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a3e65347e5acd38a18402bc222b60639d0d50266f76bb797b450828c71d7c`  
		Last Modified: Thu, 01 Apr 2021 12:45:44 GMT  
		Size: 10.6 MB (10624979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ee5f47829331d9ef32369a96363316d712305e41da1ebae5acb1afe6bcbd1f`  
		Last Modified: Thu, 01 Apr 2021 12:45:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:bed3afae2b1056fbad1a7b9d56fbebff932420e8a980068fb10c4bf805068e8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13387507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b8ccee12da4b0fa1bdc36d962d92ff4a04376637e9beaf6e4e784945e11ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:53:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:53:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:53:31 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 26 Mar 2021 05:53:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:53:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:54:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:54:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:54:12 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:54:16 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:54:21 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Fri, 26 Mar 2021 05:54:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:54:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:54:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:54:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:54:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:55:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:55:14 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:55:27 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:55:37 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:55:45 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:55:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb7d816613500788c0f13eb158c5fd78f6231a7d23540544a8b244e84513ae8`  
		Last Modified: Fri, 26 Mar 2021 05:58:36 GMT  
		Size: 302.5 KB (302534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bae6e1e4988d23946025c91dd0d3fa198434219c32c2c24ca41af5b1fd19ae`  
		Last Modified: Fri, 26 Mar 2021 05:58:36 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a1e187aa3256d1eb3e00c34ee754cdeeef160243ca9c61fda55e79def76427`  
		Last Modified: Fri, 26 Mar 2021 05:58:38 GMT  
		Size: 10.3 MB (10265875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62627650e2cb15821b38739b018e581bbf515236b463ba7db20c2871055b4b9b`  
		Last Modified: Fri, 26 Mar 2021 05:58:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1` - linux; s390x

```console
$ docker pull caddy@sha256:c4067ab1a2d33a05da3d052032444573221614e3d61bedfa21672ce29d677098
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14199974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71eba41b65371c152062463b5c0b837c7df9e8745ff9cef7acf47077e1a12e20`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:56:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:24 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 31 Mar 2021 18:56:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:28 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:28 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:28 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:28 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:28 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:30 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:31 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:31 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:31 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677a8b2d40eb111521cfa503f325130edcfec1f1d18335759af6f0e4c2042153`  
		Last Modified: Wed, 31 Mar 2021 18:57:21 GMT  
		Size: 300.8 KB (300828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1b3977b4e118165a650b8b7dc2f65e4dfd42edabf257678c0ea922af7d7ab2`  
		Last Modified: Wed, 31 Mar 2021 18:57:21 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65de8aa59970201eef2786ea94f77025aa4ee26877a536d644c07dbe17d45f04`  
		Last Modified: Wed, 31 Mar 2021 18:57:23 GMT  
		Size: 11.3 MB (11290573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fbba1efa4c623a0d77516ee26194a0bcb4d20246e5ec5e5d8bb9351158ead1`  
		Last Modified: Wed, 31 Mar 2021 18:57:21 GMT  
		Size: 155.0 B  
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
$ docker pull caddy@sha256:6eeb22834af06d78c6175701c04963deabff02d40bc9818dd980a4a1940fd3dd
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
$ docker pull caddy@sha256:90739a174e62e7c2624f9e13c300ae1a0bbd4dd22f65e7bf3738728fc5012355
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14764220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f0db44e95dc004926717fbe5536ff6c84a8b33cb1299f3207a828f6555ba94`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:38 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 13:53:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:42 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:42 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:42 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:43 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:44 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:45 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:45 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:45 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bb2b56f5f929e2a4dc7d7325b813da8143e5c9e04e10b31c96062a1c6b6dc7`  
		Last Modified: Thu, 01 Apr 2021 13:54:51 GMT  
		Size: 300.4 KB (300410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75d86528dfa0dc68505576f5dca881ac6ec4e2d2d1f722996e4e159c3ef9f12`  
		Last Modified: Thu, 01 Apr 2021 13:54:51 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f54fdea6e3e9cd7e7514b5b7238444c24373003c0eef8b9b8d73463beb7b62f`  
		Last Modified: Thu, 01 Apr 2021 13:54:53 GMT  
		Size: 11.6 MB (11645882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9224309aa0e7a8ae91bfe2da3056b90632f201d22edfa10c6a68ad0749e165e2`  
		Last Modified: Thu, 01 Apr 2021 13:54:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:1c800d34613af552185bb83c9cc5a9a0cd38787f451c4b83711bbd674244aaea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13898546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098705766700a2865c6e2f7a2d17084e261ac1a2f0da1d1f6c1ccbdcc20c2a03`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:37:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:37:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:37:39 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 31 Mar 2021 17:37:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:37:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:37:48 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:37:50 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:37:51 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:37:52 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:37:53 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 31 Mar 2021 17:37:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:37:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:38:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:38:02 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:38:03 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:38:05 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:38:14 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:38:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c9efa35742ee0a666b515a98db003c485ba9d25f69cf233de1eb63aa39c5c2`  
		Last Modified: Wed, 31 Mar 2021 17:39:06 GMT  
		Size: 300.5 KB (300517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48e60f29a99505017e416055581b9862de29e7cfe6f26070558fb74390f324e`  
		Last Modified: Wed, 31 Mar 2021 17:39:08 GMT  
		Size: 5.8 KB (5824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c996908a645bfe2c9cab1f64d06edbfeb540343c809ccbe9a6b402b1bba28024`  
		Last Modified: Wed, 31 Mar 2021 17:39:09 GMT  
		Size: 11.0 MB (10969936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8931aa62a8cba14c6dfee3aba3b7afce08b5811240c3912a1afa5319d20a42`  
		Last Modified: Wed, 31 Mar 2021 17:39:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:eaa63043acac3ff263376e0c4457d3dc81985775df976dbbd787853761bc7005
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13677725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595bb074d36d2f00bfd21d533c746c82f4a87ef97ccd29121533b0eed798df19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:12:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:12:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:12:39 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 08:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:12:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:12:48 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:12:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:12:51 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:12:52 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:53 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Thu, 01 Apr 2021 08:12:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:13:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:13:01 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:13:02 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:13:03 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:13:04 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:13:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005f2c85bbb34689fa5969c0cda8fda42d2b7848e654ff9efd67e02219a40b8f`  
		Last Modified: Thu, 01 Apr 2021 08:13:51 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d7c4a454e535a084cd7750c2ffd66ce60425166f563b6a8ac7f90dee1a6759`  
		Last Modified: Thu, 01 Apr 2021 08:13:51 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50d0ae8db26661487a79db1382dae8decc375f8add033f2e36ee304ba598f56`  
		Last Modified: Thu, 01 Apr 2021 08:13:52 GMT  
		Size: 10.9 MB (10947975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e50d54f6601d35e1dc2b6d4de04c28a5eff573b9524542e0497948c48dfeca`  
		Last Modified: Thu, 01 Apr 2021 08:13:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b6b4390de836d61962839093fb1d5d5979dae94e952eadf29fc3b54c14bcf73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13643504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ffba442e6b59579406ed8336ba2063bcb190ec8d18ab1532ca1aa675b92715`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:42:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:42:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:42:58 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 12:43:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:43:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:43:44 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:43:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:43:50 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:43:52 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:43:54 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Thu, 01 Apr 2021 12:43:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:44:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:44:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:44:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:44:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:44:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:44:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:44:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:44:26 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:44:30 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:44:38 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:44:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08584473c2f3ce7502fc1abe444e6fa79a7cc73e3e8d17f7a9907f9dc549309c`  
		Last Modified: Thu, 01 Apr 2021 12:45:41 GMT  
		Size: 300.6 KB (300621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5107f9070ac9919ca292fcdd94a304ba2a137964d1ff68207424289ef928f`  
		Last Modified: Thu, 01 Apr 2021 12:45:41 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a3e65347e5acd38a18402bc222b60639d0d50266f76bb797b450828c71d7c`  
		Last Modified: Thu, 01 Apr 2021 12:45:44 GMT  
		Size: 10.6 MB (10624979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ee5f47829331d9ef32369a96363316d712305e41da1ebae5acb1afe6bcbd1f`  
		Last Modified: Thu, 01 Apr 2021 12:45:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:bed3afae2b1056fbad1a7b9d56fbebff932420e8a980068fb10c4bf805068e8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13387507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b8ccee12da4b0fa1bdc36d962d92ff4a04376637e9beaf6e4e784945e11ade`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:53:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:53:26 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:53:31 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 26 Mar 2021 05:53:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:53:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:54:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:54:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:54:12 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:54:16 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:54:21 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Fri, 26 Mar 2021 05:54:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:54:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:54:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:54:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:54:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:55:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:55:14 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:55:27 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:55:37 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:55:45 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:55:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb7d816613500788c0f13eb158c5fd78f6231a7d23540544a8b244e84513ae8`  
		Last Modified: Fri, 26 Mar 2021 05:58:36 GMT  
		Size: 302.5 KB (302534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bae6e1e4988d23946025c91dd0d3fa198434219c32c2c24ca41af5b1fd19ae`  
		Last Modified: Fri, 26 Mar 2021 05:58:36 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a1e187aa3256d1eb3e00c34ee754cdeeef160243ca9c61fda55e79def76427`  
		Last Modified: Fri, 26 Mar 2021 05:58:38 GMT  
		Size: 10.3 MB (10265875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62627650e2cb15821b38739b018e581bbf515236b463ba7db20c2871055b4b9b`  
		Last Modified: Fri, 26 Mar 2021 05:58:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c4067ab1a2d33a05da3d052032444573221614e3d61bedfa21672ce29d677098
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14199974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71eba41b65371c152062463b5c0b837c7df9e8745ff9cef7acf47077e1a12e20`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:56:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:24 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 31 Mar 2021 18:56:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8472074e11c81292a9fc1764783c64fdc9e5909fb0711bac9544f2aac9e215757a6f42e081cd56c3be9fac7a4a7879e497b6112a7c9c5e0f43ae52f42984e9b9' ;; 		armhf)   binArch='armv6'; checksum='a947bc69e50420d99ffb5540371990db5d9800f83114ece15c72169a415d0b08c07d25ff9eb76099cd666dc9ca9dfe6662948b7a936f43cec9533c5b9bf4e91a' ;; 		armv7)   binArch='armv7'; checksum='d7b102fae8aa3b9928c55751a41d92cc0d122ca0e5e1204429ce7c2685049eba16dbb268198a791244cd3919581b7648c78aad8518d6d22f483f0bf5a323af19' ;; 		aarch64) binArch='arm64'; checksum='2e06d91729bf47d92362d7882f4e39aa896cf2d6bcb95bcab5751a51d58bf9b80fea3e2fad6c666a3a3c0e2b327c15ffc86827b13afd971868450bf1aac5d737' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a0c2a1dce40059cb6951b7ab861364d2c6857e6b1cc85816f4717886cb9f2be659b18a4a469888c1cb47160e5122188458ba819a69da979b561f12db8e8ff256' ;; 		s390x)   binArch='s390x'; checksum='d9b0c3bfbfbc5d2e8724494b5a7b7f435c6543425b27eb26c3220a0452f8e3c1e992523ec8b11f71e7751c3a45eafb193872bc154ca8e187bae8e9c26ee94b3e' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.1/caddy_2.4.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:28 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:28 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:28 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:28 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:28 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.1
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:30 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:31 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:31 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:31 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677a8b2d40eb111521cfa503f325130edcfec1f1d18335759af6f0e4c2042153`  
		Last Modified: Wed, 31 Mar 2021 18:57:21 GMT  
		Size: 300.8 KB (300828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1b3977b4e118165a650b8b7dc2f65e4dfd42edabf257678c0ea922af7d7ab2`  
		Last Modified: Wed, 31 Mar 2021 18:57:21 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65de8aa59970201eef2786ea94f77025aa4ee26877a536d644c07dbe17d45f04`  
		Last Modified: Wed, 31 Mar 2021 18:57:23 GMT  
		Size: 11.3 MB (11290573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fbba1efa4c623a0d77516ee26194a0bcb4d20246e5ec5e5d8bb9351158ead1`  
		Last Modified: Wed, 31 Mar 2021 18:57:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.1-builder`

```console
$ docker pull caddy@sha256:8cca456af26a98c600a1ce25aeed3239397c7ec39d53f2c01a3c892820a2cd52
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
$ docker pull caddy@sha256:b9ab2868e2e34ac4ddcb6d40a5ae6d608a84e43d4dfb7c66873f3b0aab88a988
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116485365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952de2871d635d8fb2d322a5adee11d50ebb7eca16886264d1169b48504c05e6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:12:47 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:12:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:12:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:12:48 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 20:14:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:14:28 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:14:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:14:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:14:29 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:50 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:50 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 13:53:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcca316e5c32a932c66cfa46736e3998e69caeb857e570566ec63ab0377044a`  
		Last Modified: Wed, 31 Mar 2021 20:22:40 GMT  
		Size: 281.3 KB (281274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b403d39c8273b612240b85430a925f80b8b5719979c21e1387246faa62bd3`  
		Last Modified: Wed, 31 Mar 2021 20:22:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d70e27e35ebcf8beb7c4148da1ce06b0c6a2f74b29fdd43ba616133688f5a6b`  
		Last Modified: Wed, 31 Mar 2021 20:22:56 GMT  
		Size: 105.7 MB (105692539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bdf7aa1b335f83aa7f89629118092911e4fd5282650af173dcf08de463314b`  
		Last Modified: Wed, 31 Mar 2021 20:22:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a96ffbefb5e94f07dc096e90dbc757d6ac77973555f7caa387321403f2ebdde`  
		Last Modified: Thu, 01 Apr 2021 13:55:02 GMT  
		Size: 6.4 MB (6387822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c221fdbee1ae80ad4d4a1682371756b429d66ced7b78673c56d1fb88d4911c4e`  
		Last Modified: Thu, 01 Apr 2021 13:55:02 GMT  
		Size: 1.3 MB (1311067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec09adb86ebc36410f8b6e2034350ac077490520281ea408c33f41bf93d9006c`  
		Last Modified: Thu, 01 Apr 2021 13:55:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:1edaea73f93d7b52ceda2f1a3c369ee71890dec64d8637dce3f2af44b447cdff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112246949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c78208a184e5ef84b7db367a17ad1886e94c34413c3bfb6b270321912bb1ca`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:28:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:28:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:28:25 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 18:44:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:44:47 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:44:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:44:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:44:54 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:05:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:25 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:27 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 04:05:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eb8dc77a7b333e6a40d00034c58c9612b3c2a7d33ea6c7dbf62e416baac7ea`  
		Last Modified: Wed, 31 Mar 2021 19:22:13 GMT  
		Size: 281.4 KB (281371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec5882b9b78ec27dce64542bb1bd7c56d4913cde0d929356e9353ea6caac515`  
		Last Modified: Wed, 31 Mar 2021 19:22:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02b4132f4d532190e4bab920cfc597ca4d398959a8793bf22e055a54a230dd9`  
		Last Modified: Wed, 31 Mar 2021 19:22:50 GMT  
		Size: 101.9 MB (101896075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac885759424a47ac2b08ab253206844465a38311eb822180b7167f46dabc078`  
		Last Modified: Wed, 31 Mar 2021 19:22:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9e34ed7b78eaaf51d4ca1c99bffab072d0995cb3ff67c99b4ca0a46a6962a`  
		Last Modified: Thu, 01 Apr 2021 04:06:19 GMT  
		Size: 6.2 MB (6225082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1e0b778b6df662938dc29e74beda5bb6cfd8b6fc375534ff870a4b283ecdb1`  
		Last Modified: Thu, 01 Apr 2021 04:06:18 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dec733894d338a9ffee02f89794efb9376d20926653e1c375819ab933673c1`  
		Last Modified: Thu, 01 Apr 2021 04:06:17 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:699989d99b1f4fe78ced6c6828f36c525e50fffbadb6aab9385565dcc3a8d8ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111180348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79738346995def80e3aa79e16fff0c54fbd54e5369f5652e70559c14e6bcc65b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:43:30 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:43:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:43:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 11:43:35 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 01 Apr 2021 11:56:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 11:56:18 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 11:56:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 11:56:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 11:56:23 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:54 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:54 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 14:30:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:31:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60891e1263b2984a8f23c01f468bc717e4ed53012265c3d898ebdde9178b3f3`  
		Last Modified: Thu, 01 Apr 2021 13:00:26 GMT  
		Size: 280.5 KB (280526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9c885d816d12af70fab6cfcb656be2aaec3481f10aa9b8381e4c8b1ddb8c2f`  
		Last Modified: Thu, 01 Apr 2021 13:00:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cad23d792d56d118ac89b52a5fadbdd61c1c8645a393ef96ffed663204648d`  
		Last Modified: Thu, 01 Apr 2021 13:00:56 GMT  
		Size: 101.7 MB (101697417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72f4c132557c92c7cfe80943a3d499da3022a16063bc3c4b75c6aac48e50fc9`  
		Last Modified: Thu, 01 Apr 2021 13:00:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7c27b474a5992a2ea4ebb6a303285127f2cfe56a282365d757cc366dda7f7e`  
		Last Modified: Thu, 01 Apr 2021 14:31:45 GMT  
		Size: 5.6 MB (5558134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54daab929cc3e4129034530ca7f558968d7b4a6ac008eb818761bc456ccdeb4`  
		Last Modified: Thu, 01 Apr 2021 14:31:44 GMT  
		Size: 1.2 MB (1219447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e15c7f633338ccf72beefcab932e79802ce2ff75979826c679bdcf24e9cd045`  
		Last Modified: Thu, 01 Apr 2021 14:31:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d2644c5fbdbabad025566fb5b1e621784dde51b058296ff52ce7a2454afdb105
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111681194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454c666217d26e782e79115fd7e2c496d2ae67d25cd06f4ec1d17a77c6ffa4b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:48:27 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:48:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:48:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:48:35 GMT
ENV GOLANG_VERSION=1.16.2
# Fri, 26 Mar 2021 00:51:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 00:51:16 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 00:51:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:51:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 00:51:22 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:59 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:12:00 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 26 Mar 2021 16:12:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:12:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:12:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ff46675bd06010716fe2b0b0ec0f47c75a764178583b4fb76a94252e65ff44`  
		Last Modified: Fri, 26 Mar 2021 01:01:52 GMT  
		Size: 281.5 KB (281481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc63843dca3ec418c6b57e99b6f88cb70c3cbc1cbcc82978df5f62fc0e991366`  
		Last Modified: Fri, 26 Mar 2021 01:01:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7507b63d90c6373bf5f4854f6bf7c294b4faf52954b34a23b1c33fec5c6f22`  
		Last Modified: Fri, 26 Mar 2021 01:02:24 GMT  
		Size: 101.0 MB (101011501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d06fd061698bb804ea6448e3c6a97e273b3f96443c2281102e21f35aaaa2bf7`  
		Last Modified: Fri, 26 Mar 2021 01:01:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa283540ec18f8b2cf9d1a72ae9577008e707d3bdf4f7faa0ffaa296a06ece6`  
		Last Modified: Fri, 26 Mar 2021 16:12:44 GMT  
		Size: 6.5 MB (6474041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ed8fa69c6d9f4a9a4c661af9198a253e368bb9087142915e1d50bbbdd696dd`  
		Last Modified: Fri, 26 Mar 2021 16:12:45 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c76f96790bd896ac7f3bb09d643aa14c866132a976483de0ab7d4f2e436cf3b`  
		Last Modified: Fri, 26 Mar 2021 16:12:43 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1ea2d9f9195c6145c5ee34e986a096ca761500688a7f3f5bbac6023f18b0fd37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110575715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fe4217fbbb0faba83cb7c0c63ff1b62c13b07f0f55d7ac3a8fa58e5413eb2f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:45:24 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:45:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:45:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:45:52 GMT
ENV GOLANG_VERSION=1.16.2
# Fri, 26 Mar 2021 00:48:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 00:48:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 00:48:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:48:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 00:48:56 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:56:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:56:23 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:56:46 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 26 Mar 2021 05:56:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:57:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:57:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee939b03e1bace56e69c95d0dc49998852768838bdc34268f741f12112ccbeb`  
		Last Modified: Fri, 26 Mar 2021 01:03:42 GMT  
		Size: 283.4 KB (283403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c4c75228ef872078f04a251465173c8c1f2ac433aa142832ec85ae5eb9c19e`  
		Last Modified: Fri, 26 Mar 2021 01:03:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e591d09f3336615c7aef423b970a983c3d3474dca3c3cf6781c5b59daad2912`  
		Last Modified: Fri, 26 Mar 2021 01:05:43 GMT  
		Size: 99.5 MB (99484784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300812994d50d48e4b6d8e7c9d933f3bf24a5b0f49fed26712f20cafd7099b35`  
		Last Modified: Fri, 26 Mar 2021 01:03:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d07c5c7c22b481e3eb5842e23549104090a79e40986e8626d2e1e7546ce40fa`  
		Last Modified: Fri, 26 Mar 2021 05:58:52 GMT  
		Size: 6.8 MB (6823205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333a25deafb6cb51967bbd58438643c674032e93aaef192b920e0d194c08e40f`  
		Last Modified: Fri, 26 Mar 2021 05:58:50 GMT  
		Size: 1.2 MB (1170493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9798c40bd61fa5d14606ad02fed17bc7e7ce82f6bc5f67d37cc52d0464ff4dde`  
		Last Modified: Fri, 26 Mar 2021 05:58:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:64917b325999309920e1418218c0e8bc0f6e5db087832d55f679bebb8fb5c8e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115408574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b57100f0f63da50588830889e4c6d4d35b6fa831c5be5578f00ff1593dee634`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:32:50 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:32:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:32:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:32:51 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 18:34:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:34:27 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:34:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:34:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:34:28 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:37 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 31 Mar 2021 18:56:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c9dd6f50e848494b74d743acede663c4566d6c904f83c807df6ed135c0bac2`  
		Last Modified: Wed, 31 Mar 2021 18:40:22 GMT  
		Size: 281.7 KB (281696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a3302e682073b38a23dae31007fd1b72ed66261ca926cc100f29e177732a0a`  
		Last Modified: Wed, 31 Mar 2021 18:40:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4a9647efdfd2fe83835843ee761ff6c800604a0a2514db1cc014e18fa55664`  
		Last Modified: Wed, 31 Mar 2021 18:40:34 GMT  
		Size: 104.8 MB (104787299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5d3e1bba60e9d306da5ecd18bbbf586943da4bdc6d87c1c20338b0371f3552`  
		Last Modified: Wed, 31 Mar 2021 18:40:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b3555e36eafafa84632965d97cf7686e8a2a710a406fb1581a621db42426c`  
		Last Modified: Wed, 31 Mar 2021 18:57:31 GMT  
		Size: 6.5 MB (6471841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53c7c75af0ae1e170542713c49e25ad66ab82311394ce727ca7f4028e36fc1c`  
		Last Modified: Wed, 31 Mar 2021 18:57:31 GMT  
		Size: 1.3 MB (1264433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfffff286c04107f6be28450cc880227216c7f50643f50bb4249619690a9e12b`  
		Last Modified: Wed, 31 Mar 2021 18:57:28 GMT  
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
$ docker pull caddy@sha256:b27396c0153431153d7a54dc7b9c83763134431a30c7b90b42e771e1db7d48e9
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
$ docker pull caddy@sha256:b9ab2868e2e34ac4ddcb6d40a5ae6d608a84e43d4dfb7c66873f3b0aab88a988
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116485365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952de2871d635d8fb2d322a5adee11d50ebb7eca16886264d1169b48504c05e6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:12:47 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:12:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:12:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:12:48 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 20:14:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:14:28 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:14:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:14:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:14:29 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:50 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:50 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 13:53:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcca316e5c32a932c66cfa46736e3998e69caeb857e570566ec63ab0377044a`  
		Last Modified: Wed, 31 Mar 2021 20:22:40 GMT  
		Size: 281.3 KB (281274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b403d39c8273b612240b85430a925f80b8b5719979c21e1387246faa62bd3`  
		Last Modified: Wed, 31 Mar 2021 20:22:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d70e27e35ebcf8beb7c4148da1ce06b0c6a2f74b29fdd43ba616133688f5a6b`  
		Last Modified: Wed, 31 Mar 2021 20:22:56 GMT  
		Size: 105.7 MB (105692539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bdf7aa1b335f83aa7f89629118092911e4fd5282650af173dcf08de463314b`  
		Last Modified: Wed, 31 Mar 2021 20:22:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a96ffbefb5e94f07dc096e90dbc757d6ac77973555f7caa387321403f2ebdde`  
		Last Modified: Thu, 01 Apr 2021 13:55:02 GMT  
		Size: 6.4 MB (6387822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c221fdbee1ae80ad4d4a1682371756b429d66ced7b78673c56d1fb88d4911c4e`  
		Last Modified: Thu, 01 Apr 2021 13:55:02 GMT  
		Size: 1.3 MB (1311067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec09adb86ebc36410f8b6e2034350ac077490520281ea408c33f41bf93d9006c`  
		Last Modified: Thu, 01 Apr 2021 13:55:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:1edaea73f93d7b52ceda2f1a3c369ee71890dec64d8637dce3f2af44b447cdff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112246949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c78208a184e5ef84b7db367a17ad1886e94c34413c3bfb6b270321912bb1ca`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:28:21 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:28:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:28:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:28:25 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 18:44:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:44:47 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:44:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:44:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:44:54 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:05:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:25 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:27 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 04:05:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eb8dc77a7b333e6a40d00034c58c9612b3c2a7d33ea6c7dbf62e416baac7ea`  
		Last Modified: Wed, 31 Mar 2021 19:22:13 GMT  
		Size: 281.4 KB (281371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec5882b9b78ec27dce64542bb1bd7c56d4913cde0d929356e9353ea6caac515`  
		Last Modified: Wed, 31 Mar 2021 19:22:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02b4132f4d532190e4bab920cfc597ca4d398959a8793bf22e055a54a230dd9`  
		Last Modified: Wed, 31 Mar 2021 19:22:50 GMT  
		Size: 101.9 MB (101896075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac885759424a47ac2b08ab253206844465a38311eb822180b7167f46dabc078`  
		Last Modified: Wed, 31 Mar 2021 19:22:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9e34ed7b78eaaf51d4ca1c99bffab072d0995cb3ff67c99b4ca0a46a6962a`  
		Last Modified: Thu, 01 Apr 2021 04:06:19 GMT  
		Size: 6.2 MB (6225082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1e0b778b6df662938dc29e74beda5bb6cfd8b6fc375534ff870a4b283ecdb1`  
		Last Modified: Thu, 01 Apr 2021 04:06:18 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dec733894d338a9ffee02f89794efb9376d20926653e1c375819ab933673c1`  
		Last Modified: Thu, 01 Apr 2021 04:06:17 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:699989d99b1f4fe78ced6c6828f36c525e50fffbadb6aab9385565dcc3a8d8ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111180348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79738346995def80e3aa79e16fff0c54fbd54e5369f5652e70559c14e6bcc65b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:43:30 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:43:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:43:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 11:43:35 GMT
ENV GOLANG_VERSION=1.16.2
# Thu, 01 Apr 2021 11:56:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 11:56:18 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 11:56:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 11:56:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 11:56:23 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:54 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:54 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Thu, 01 Apr 2021 14:30:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:31:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60891e1263b2984a8f23c01f468bc717e4ed53012265c3d898ebdde9178b3f3`  
		Last Modified: Thu, 01 Apr 2021 13:00:26 GMT  
		Size: 280.5 KB (280526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9c885d816d12af70fab6cfcb656be2aaec3481f10aa9b8381e4c8b1ddb8c2f`  
		Last Modified: Thu, 01 Apr 2021 13:00:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cad23d792d56d118ac89b52a5fadbdd61c1c8645a393ef96ffed663204648d`  
		Last Modified: Thu, 01 Apr 2021 13:00:56 GMT  
		Size: 101.7 MB (101697417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72f4c132557c92c7cfe80943a3d499da3022a16063bc3c4b75c6aac48e50fc9`  
		Last Modified: Thu, 01 Apr 2021 13:00:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7c27b474a5992a2ea4ebb6a303285127f2cfe56a282365d757cc366dda7f7e`  
		Last Modified: Thu, 01 Apr 2021 14:31:45 GMT  
		Size: 5.6 MB (5558134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54daab929cc3e4129034530ca7f558968d7b4a6ac008eb818761bc456ccdeb4`  
		Last Modified: Thu, 01 Apr 2021 14:31:44 GMT  
		Size: 1.2 MB (1219447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e15c7f633338ccf72beefcab932e79802ce2ff75979826c679bdcf24e9cd045`  
		Last Modified: Thu, 01 Apr 2021 14:31:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d2644c5fbdbabad025566fb5b1e621784dde51b058296ff52ce7a2454afdb105
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111681194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454c666217d26e782e79115fd7e2c496d2ae67d25cd06f4ec1d17a77c6ffa4b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:48:27 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:48:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:48:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:48:35 GMT
ENV GOLANG_VERSION=1.16.2
# Fri, 26 Mar 2021 00:51:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 00:51:16 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 00:51:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:51:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 00:51:22 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:59 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:12:00 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 26 Mar 2021 16:12:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:12:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:12:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ff46675bd06010716fe2b0b0ec0f47c75a764178583b4fb76a94252e65ff44`  
		Last Modified: Fri, 26 Mar 2021 01:01:52 GMT  
		Size: 281.5 KB (281481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc63843dca3ec418c6b57e99b6f88cb70c3cbc1cbcc82978df5f62fc0e991366`  
		Last Modified: Fri, 26 Mar 2021 01:01:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7507b63d90c6373bf5f4854f6bf7c294b4faf52954b34a23b1c33fec5c6f22`  
		Last Modified: Fri, 26 Mar 2021 01:02:24 GMT  
		Size: 101.0 MB (101011501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d06fd061698bb804ea6448e3c6a97e273b3f96443c2281102e21f35aaaa2bf7`  
		Last Modified: Fri, 26 Mar 2021 01:01:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa283540ec18f8b2cf9d1a72ae9577008e707d3bdf4f7faa0ffaa296a06ece6`  
		Last Modified: Fri, 26 Mar 2021 16:12:44 GMT  
		Size: 6.5 MB (6474041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ed8fa69c6d9f4a9a4c661af9198a253e368bb9087142915e1d50bbbdd696dd`  
		Last Modified: Fri, 26 Mar 2021 16:12:45 GMT  
		Size: 1.2 MB (1201558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c76f96790bd896ac7f3bb09d643aa14c866132a976483de0ab7d4f2e436cf3b`  
		Last Modified: Fri, 26 Mar 2021 16:12:43 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1ea2d9f9195c6145c5ee34e986a096ca761500688a7f3f5bbac6023f18b0fd37
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110575715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fe4217fbbb0faba83cb7c0c63ff1b62c13b07f0f55d7ac3a8fa58e5413eb2f2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:45:24 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:45:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:45:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:45:52 GMT
ENV GOLANG_VERSION=1.16.2
# Fri, 26 Mar 2021 00:48:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 00:48:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 00:48:30 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:48:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 00:48:56 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:56:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:56:23 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:56:46 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Fri, 26 Mar 2021 05:56:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:57:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:57:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee939b03e1bace56e69c95d0dc49998852768838bdc34268f741f12112ccbeb`  
		Last Modified: Fri, 26 Mar 2021 01:03:42 GMT  
		Size: 283.4 KB (283403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c4c75228ef872078f04a251465173c8c1f2ac433aa142832ec85ae5eb9c19e`  
		Last Modified: Fri, 26 Mar 2021 01:03:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e591d09f3336615c7aef423b970a983c3d3474dca3c3cf6781c5b59daad2912`  
		Last Modified: Fri, 26 Mar 2021 01:05:43 GMT  
		Size: 99.5 MB (99484784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300812994d50d48e4b6d8e7c9d933f3bf24a5b0f49fed26712f20cafd7099b35`  
		Last Modified: Fri, 26 Mar 2021 01:03:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d07c5c7c22b481e3eb5842e23549104090a79e40986e8626d2e1e7546ce40fa`  
		Last Modified: Fri, 26 Mar 2021 05:58:52 GMT  
		Size: 6.8 MB (6823205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333a25deafb6cb51967bbd58438643c674032e93aaef192b920e0d194c08e40f`  
		Last Modified: Fri, 26 Mar 2021 05:58:50 GMT  
		Size: 1.2 MB (1170493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9798c40bd61fa5d14606ad02fed17bc7e7ce82f6bc5f67d37cc52d0464ff4dde`  
		Last Modified: Fri, 26 Mar 2021 05:58:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:64917b325999309920e1418218c0e8bc0f6e5db087832d55f679bebb8fb5c8e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115408574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b57100f0f63da50588830889e4c6d4d35b6fa831c5be5578f00ff1593dee634`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:32:50 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:32:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:32:51 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:32:51 GMT
ENV GOLANG_VERSION=1.16.2
# Wed, 31 Mar 2021 18:34:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.2.src.tar.gz'; 	sha256='37ca14287a23cb8ba2ac3f5c3dd8adbc1f7a54b9701a57824bf19a0b271f83ea'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:34:27 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:34:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:34:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:34:28 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:37 GMT
ENV CADDY_VERSION=v2.4.0-beta.1
# Wed, 31 Mar 2021 18:56:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c9dd6f50e848494b74d743acede663c4566d6c904f83c807df6ed135c0bac2`  
		Last Modified: Wed, 31 Mar 2021 18:40:22 GMT  
		Size: 281.7 KB (281696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a3302e682073b38a23dae31007fd1b72ed66261ca926cc100f29e177732a0a`  
		Last Modified: Wed, 31 Mar 2021 18:40:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4a9647efdfd2fe83835843ee761ff6c800604a0a2514db1cc014e18fa55664`  
		Last Modified: Wed, 31 Mar 2021 18:40:34 GMT  
		Size: 104.8 MB (104787299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5d3e1bba60e9d306da5ecd18bbbf586943da4bdc6d87c1c20338b0371f3552`  
		Last Modified: Wed, 31 Mar 2021 18:40:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6b3555e36eafafa84632965d97cf7686e8a2a710a406fb1581a621db42426c`  
		Last Modified: Wed, 31 Mar 2021 18:57:31 GMT  
		Size: 6.5 MB (6471841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53c7c75af0ae1e170542713c49e25ad66ab82311394ce727ca7f4028e36fc1c`  
		Last Modified: Wed, 31 Mar 2021 18:57:31 GMT  
		Size: 1.3 MB (1264433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfffff286c04107f6be28450cc880227216c7f50643f50bb4249619690a9e12b`  
		Last Modified: Wed, 31 Mar 2021 18:57:28 GMT  
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
$ docker pull caddy@sha256:a18e9c84fb32bae7eeaab4b048f10c4ec8797e4641f8d7d5f75d35e11282d0e3
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
$ docker pull caddy@sha256:629c5800ccf51df482a4e63266e4570de3e573e862d902398b03cbfca2212b4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e073d63a624f18bd8e2f94b9e84715e5a33a817db19afa42afc8ea95e59d568`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:17 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:24 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc82ca1670c70e5b605729b271409acba02ca26c3f669bf1d95a067fb853a90`  
		Last Modified: Thu, 01 Apr 2021 13:54:20 GMT  
		Size: 300.0 KB (300021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d66f69260e9358ba74c27e0ed110b9ff7781c5f90d5d01f86d6ef289834382`  
		Last Modified: Thu, 01 Apr 2021 13:54:17 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b38557b1fd80a7712b7263f0896f076afdeb9f25f68a79e288b87490aa3047`  
		Last Modified: Thu, 01 Apr 2021 13:54:19 GMT  
		Size: 11.6 MB (11622380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37d6fba45d5f1633f00b6a9d204abacad2a6918dc355706fe0decc0bc4e565`  
		Last Modified: Thu, 01 Apr 2021 13:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b57cdc61b54865a7ff2ea4ef9d16458537d40e0dc25559d6540111874abbe4ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88293e19906b6b2275ff6e127e29960b1fdf0cf0c4baa4bbce4ea297e90db731`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:36:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:36:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:36:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 17:36:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:36:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:36:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:36:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:36:56 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 17:36:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:36:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:37:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:37:07 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:37:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:37:10 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:37:11 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:37:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1532456df32c320ccd3c9ff5433c9e44d873ef87a0dc9fc29f9cf256b517eb4`  
		Last Modified: Wed, 31 Mar 2021 17:38:50 GMT  
		Size: 300.1 KB (300103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263f61714ef61a0c59bef8e70bc49a741a357b0a0fc556b44f8344df37ea0f8`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818002dab28746359de43d5a88d06c77cc3a353c838e15c6b6a67d48352cc5c0`  
		Last Modified: Wed, 31 Mar 2021 17:38:54 GMT  
		Size: 10.9 MB (10944835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979a3c808bf5c07c668f5966a15458dbfe9aba5aa7d761e690dd3a5cadf45eb`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6d510324512c20fc0d40aeb8b6e5b98255c857ad2dee894b6cb6e66f0231cf9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42db38da968682707e6cf0fabb16f93770388907d8a208fca0db74cae3183ba2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:11:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:11:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:11:48 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 08:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:11:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:11:56 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:11:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:11:58 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:11:59 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 08:12:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:12:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:12:09 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:12:11 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:12:13 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:12:15 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:12:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547b5d01ba24abc02b4f05f8134bfb156ce1840f496ed03a1316c882625bd41f`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 299.2 KB (299199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a883a914d37801ae97b0fac82c62e4f70ef4c92fc53417a91a23b2e69d36d9bb`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475143e7b89d1a36700916ec3c8f0caae9b57d5cd9ba187b9f3fd5d9a71eddcf`  
		Last Modified: Thu, 01 Apr 2021 08:13:38 GMT  
		Size: 10.9 MB (10925346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79cdab22a3397c4a98f63a7e96c51881033744b1f198c4984072e7303e9f73`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1c3e6c1b947162789190f9215b56c517caa5c48bd5d09f9753c6ff105ece8ea4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d36a254c95d4ad655ca159d67b79ad8ca4498f82a3c127340a7b5be09e213b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:40:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:40:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:40:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 12:40:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:40:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:40:35 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:40:38 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:40:44 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:40:49 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:40:53 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 12:40:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:40:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:40:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:40:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:40:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:41:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:41:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:41:05 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:41:08 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:41:12 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:41:18 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1fbebcb85e1b4f7457195688308678e46184f78ec8402dcd4eb0992700541`  
		Last Modified: Thu, 01 Apr 2021 12:45:24 GMT  
		Size: 300.3 KB (300333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c34c85964e1be21b929d726522dfd448c029aaf7acd32bf5342ff93070124bd`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c657d5761128c010be222b8ddea92ceba700a3c76afb7704c9d436bbb5582c1`  
		Last Modified: Thu, 01 Apr 2021 12:45:27 GMT  
		Size: 10.6 MB (10598978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90c89f24747de4d19b1c83875e0072662bfe7ce4c5f4e15c551d907b212ebc`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d8ff14acdf013e9a2df27d95f3326bf7175307a04e9e6f7a40b840bf813898ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63b8a5e4185f59e46edc1e47b15d592327b0c3b8867d3edd3be3a9b3dea5522`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:49:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:49:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:49:51 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:50:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:50:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:50:24 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:50:30 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:50:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 05:50:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:50:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:50:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:50:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:50:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:51:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:51:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:51:24 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:51:30 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:51:35 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:51:40 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:51:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69ab62cc22d6fb5ba7a45731c0b8f378026c7c711d7d48946bfe7c69eae199`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 302.3 KB (302337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9767f7d2aec64fa7c89aa12c9b2b14b03dbe10e20cf53279a88f5009dd2c7841`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502018de7a2dcf0f08830ebcce7c073c9a9db95ecf366d96d44c7a76ba032edc`  
		Last Modified: Fri, 26 Mar 2021 05:58:02 GMT  
		Size: 10.2 MB (10241383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61815e7304b64383c90b6c68c7220f40b74c932f3dd3cfd44b04fed05920aec`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9d992badb7530225182676af12ae945f5f2de2f5ad7d3946b397892a6de4c123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c8a68869d0806c29e6c2c9c655d3e9085af285c6c24ea651ad3bdffd714e38`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:55:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:00 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:05 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:06 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:08 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8eb19b6319d0b09121581759094c3eb58e5574e2063affb6c42c0e1a1937a0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd6e269a873b8a21e2787b0ea05662c0f2676aa9043f52b8884081965be7112`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f6a8a7e19cb11edbda771ce361181202915f4760cdaef5e290b1758cc7b88c`  
		Last Modified: Wed, 31 Mar 2021 18:57:02 GMT  
		Size: 11.3 MB (11272066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec92d2dcab4ee41e4e626d8b360a6feff3822db894894865a36bbe9cfc759df0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:803eb2fbf7bc2389c531d241d9596982a84cb74a9d37fc2659e95c3f8ebeccaf
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
$ docker pull caddy@sha256:a9cf52bbabc8864aa2bb39cc3b30034060f8b5cfea57a24af5d59fb712a2363d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119514478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972e1302f4350651067d073928bc15bcd5b0219ea111332de1bb9a3eb2af6800`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:14:43 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:14:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:14:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:18:53 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 20:20:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:20:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:20:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:20:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:20:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbbf235a55c104bafc6765f3c92a36489a596041551360d566152f2af01b59`  
		Last Modified: Wed, 31 Mar 2021 20:22:25 GMT  
		Size: 280.9 KB (280881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f184a059628efa0b05f924f5b1e223377ebd57cdec0597912aabcd4b2129b`  
		Last Modified: Wed, 31 Mar 2021 20:23:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec81731eed009f8d947489208d3bc2fe161411bd6ad9543fc2af27bb229d352`  
		Last Modified: Wed, 31 Mar 2021 20:26:05 GMT  
		Size: 106.8 MB (106811699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec2af768a6dad08fb2f9bf5396591d7ab1b7bff816d42c96f7c5169ab05502`  
		Last Modified: Wed, 31 Mar 2021 20:25:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d41b37a714ddeeea16e8fb5e39787ea218dc37873bcc66c101e72177214f54`  
		Last Modified: Thu, 01 Apr 2021 13:54:35 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30dccfb57aae7671a60a9a97a865cdfb7223a51d8d176ca6c833f95a3d0c3`  
		Last Modified: Thu, 01 Apr 2021 13:54:36 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c224dde9c00bfc5be3cc063759e6e39bb2d1586ad856299e4dc5edcbce99ea0d`  
		Last Modified: Thu, 01 Apr 2021 13:54:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:528de32f232e1620d7a832171f2de05db14a38b0367b601508a3554ee39609d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cb88e37729e6535c0e5d37dd52aabf2191db2fc10d3a2d5cc2befb4a3547e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:45:17 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:45:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:45:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:13:42 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 19:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 19:21:40 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 19:21:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 19:21:45 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:04:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:00 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:02 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 04:05:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa6796eed51884cd0436f134281af9489342ecf256aec0b31ca83f254ccd0d1`  
		Last Modified: Wed, 31 Mar 2021 19:23:16 GMT  
		Size: 281.0 KB (280979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c043dc86373f816c29db582d9bddada9a00eeb3812a357a2dfd8e3f68d9a413`  
		Last Modified: Wed, 31 Mar 2021 19:23:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031875ceeaab9b0b96a47b7ed9ec2a0098a9d8662d1c2a57785eb95dbf36d419`  
		Last Modified: Wed, 31 Mar 2021 19:25:23 GMT  
		Size: 102.7 MB (102671786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15870044ac3cd6474d13a6fd94871020ad8801d56fa4387bb9507968da9b093d`  
		Last Modified: Wed, 31 Mar 2021 19:24:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa970c15af3c0912614e0bd697d3329aa1d7f2e98e13f86227bec493367295`  
		Last Modified: Thu, 01 Apr 2021 04:06:04 GMT  
		Size: 7.9 MB (7929419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231389672c1c8c7a9fd39092006eca8983b058e9edc5f0d04bf43bc3f9dea700`  
		Last Modified: Thu, 01 Apr 2021 04:06:02 GMT  
		Size: 1.2 MB (1221595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efaab869ceebc633c179dc051159fb587f7bb30890e765be3f630558cc9933c`  
		Last Modified: Thu, 01 Apr 2021 04:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:673ccce087f4fef545f63f971a0738dbb551fa5872c1742be37a89daded09f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83363f4d6122099578251753b8d8052a348737a2593393b43b431795fcb64292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:56:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:56:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:56:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:36:58 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 01 Apr 2021 12:59:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 12:59:20 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 12:59:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:59:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 12:59:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:27 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 14:30:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:30:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b725919da0175e4c01c41441c29fff6f5ec6c0c4e37417f70120f08f96acfc`  
		Last Modified: Thu, 01 Apr 2021 13:01:16 GMT  
		Size: 280.1 KB (280073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1f51d8714e34d5e746102b7176e77e8142ecf71f4c68d82354285a0bd6d16`  
		Last Modified: Thu, 01 Apr 2021 13:01:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9a84aba5c985724e2f9d0049434534ed654c74b46945f50cc2af08567b9b6`  
		Last Modified: Thu, 01 Apr 2021 13:03:20 GMT  
		Size: 102.5 MB (102462580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc655d7de77ca2ce887998caba1ec52a0bd3f8aa5453bb583ba83449613e96c5`  
		Last Modified: Thu, 01 Apr 2021 13:02:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c177cdf044a6b683b9c1a95121917806970172353334871227cb79e618bc0b1`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1d6a25abce1b9f81c345e1c2ac0149a173ffdcdca04c5ffd9a450903aa2d2`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 1.2 MB (1219450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1bc2f6f317df593b6011ce90f58a1234127d7f78cf8121f8972f79d564b69`  
		Last Modified: Thu, 01 Apr 2021 14:31:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e8c8a0956ea40a17133ef7055aa4cd1076f944342cddf3665d91c8addbe8effb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8892c660131d71ee38d69f56f72c5e98aed80471af824bd1ceda7b5a08c2ce4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:51:33 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:57:28 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:00:54 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:01:02 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:11:38 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 16:11:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:11:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:11:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:11:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f941853f4c183d3b0a653353ba7515088ae2488b01a0ca6bddaa6f1dcc062d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 281.2 KB (281215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4be3bf1d235e013412b55ba1e824da6cfebaf80d284481002d2aa00718563d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc4f0c823675028e8e8caed39be27c63850615a4394ab508faf5b4ed3a9fc3`  
		Last Modified: Fri, 26 Mar 2021 01:04:37 GMT  
		Size: 102.1 MB (102143643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ce0d84f3cb43a1eb06c18a87965b988275ab2c863043b96032d5d4b94d5db`  
		Last Modified: Fri, 26 Mar 2021 01:04:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6274beb5e6ef4051612c2bcfadde952a3caceb7145e9f6d61ce0b818f2e4f7`  
		Last Modified: Fri, 26 Mar 2021 16:12:33 GMT  
		Size: 8.5 MB (8500012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880cf9840fe472a748b59dbd60483c321b780ac76a1906aafe3c082bfd41496d`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 1.2 MB (1201557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d154a0032206067bed60392933ce1a8bab8e7cd48226b92f0f589d7f1bd746`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:b84ae4910f796380e57d7daac89af75d8012094746a88fa467d97bafcdb11fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113985368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b7945ba534d20ab228061857652036740c946d79102221e87b9fb0ea979254`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:50:54 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:58:55 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:01:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:01:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:01:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:02:00 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:52:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:52:17 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:52:23 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:52:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:52:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:52:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22fc023a51f1560551f97595c0d26436968276b81fd2119cb972238aff23fb6`  
		Last Modified: Fri, 26 Mar 2021 01:06:49 GMT  
		Size: 283.2 KB (283209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b5b049d7abfca6a07577171113a612a55eb6f864651563d204b02fb5c4e60`  
		Last Modified: Fri, 26 Mar 2021 01:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db853427f2ec5049b1f9079b25be4c8117deaa1fcac132410fa8c0b1deb720c8`  
		Last Modified: Fri, 26 Mar 2021 01:12:48 GMT  
		Size: 100.8 MB (100803535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d927b70afd72e9dd133e5d57a45143c8e8ebceefa2dfc3a7fc1bd8e1b9ce83d8`  
		Last Modified: Fri, 26 Mar 2021 01:12:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf5bc1fa9c61f972e646bacb633a53efd7d173b4d79b2efd32f923d503d50b`  
		Last Modified: Fri, 26 Mar 2021 05:58:21 GMT  
		Size: 8.9 MB (8921440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6874c8aee6bfafc6a12719998f12ce1dcf70d8a61da3dd914f9c791808221`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0826f628855fe686aafb0d3423a1c5258fcb72287998561865187f7e7d4f0`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:e7648a8c6fc41f80b2eb8da973742a7485f479cb4f57dcb04d738e8800f5b64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118389839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8b0338c771c7f370f6460e6a444505905acc419685f5c8d35648800e50d8c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:34:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:34:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:34:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:38:18 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 18:39:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:39:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:39:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:39:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:39:47 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:15 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb296d6fc71cd9057e3d03d0ea4ebe30a620f7c6ce57eb78f4c137e77a9a47`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 281.4 KB (281355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783b7db1c405d51f50a261ae252c97941c44ffeb93cb10c2e2bdd458296774a`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb58064707977215f9632cdb206eaec9d63534f602e5682c22634dcfbb2cbd5`  
		Last Modified: Wed, 31 Mar 2021 18:42:02 GMT  
		Size: 105.9 MB (105923109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273a64a6b34c09c3baa0d7e2dc15a36980a72e658c1570903625ebac61f7f16`  
		Last Modified: Wed, 31 Mar 2021 18:41:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadae105e5bbdd611f262c9d81668d5b3251f7c246bd9bd444ecd4c88b936326`  
		Last Modified: Wed, 31 Mar 2021 18:57:12 GMT  
		Size: 8.4 MB (8352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7739fc64956105cdc380f5c596d98e8b490d06ca763be1a88849e780ddcc74`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 1.3 MB (1264435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad00fa157eebdd61affab09a5b4d3ba310bf443dca82d624ae508b390df30ea6`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:fe5e31b0b4e73341e2002706c4b0fc665dc25f118fee2497eeb4c213283a94c4
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
$ docker pull caddy@sha256:a9cf52bbabc8864aa2bb39cc3b30034060f8b5cfea57a24af5d59fb712a2363d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119514478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972e1302f4350651067d073928bc15bcd5b0219ea111332de1bb9a3eb2af6800`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 20:14:43 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 20:14:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 20:14:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:18:53 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 20:20:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 20:20:24 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 20:20:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 20:20:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 20:20:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 13:53:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 13:53:29 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 13:53:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 13:53:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 13:53:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cbbf235a55c104bafc6765f3c92a36489a596041551360d566152f2af01b59`  
		Last Modified: Wed, 31 Mar 2021 20:22:25 GMT  
		Size: 280.9 KB (280881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f184a059628efa0b05f924f5b1e223377ebd57cdec0597912aabcd4b2129b`  
		Last Modified: Wed, 31 Mar 2021 20:23:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec81731eed009f8d947489208d3bc2fe161411bd6ad9543fc2af27bb229d352`  
		Last Modified: Wed, 31 Mar 2021 20:26:05 GMT  
		Size: 106.8 MB (106811699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec2af768a6dad08fb2f9bf5396591d7ab1b7bff816d42c96f7c5169ab05502`  
		Last Modified: Wed, 31 Mar 2021 20:25:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d41b37a714ddeeea16e8fb5e39787ea218dc37873bcc66c101e72177214f54`  
		Last Modified: Thu, 01 Apr 2021 13:54:35 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e30dccfb57aae7671a60a9a97a865cdfb7223a51d8d176ca6c833f95a3d0c3`  
		Last Modified: Thu, 01 Apr 2021 13:54:36 GMT  
		Size: 1.3 MB (1311071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c224dde9c00bfc5be3cc063759e6e39bb2d1586ad856299e4dc5edcbce99ea0d`  
		Last Modified: Thu, 01 Apr 2021 13:54:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:528de32f232e1620d7a832171f2de05db14a38b0367b601508a3554ee39609d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114709152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15cb88e37729e6535c0e5d37dd52aabf2191db2fc10d3a2d5cc2befb4a3547e3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:45:17 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:45:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:45:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:13:42 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 19:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 19:21:40 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 19:21:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 19:21:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 19:21:45 GMT
WORKDIR /go
# Thu, 01 Apr 2021 04:04:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 04:05:00 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 04:05:02 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 04:05:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 04:05:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 04:05:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 04:05:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa6796eed51884cd0436f134281af9489342ecf256aec0b31ca83f254ccd0d1`  
		Last Modified: Wed, 31 Mar 2021 19:23:16 GMT  
		Size: 281.0 KB (280979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c043dc86373f816c29db582d9bddada9a00eeb3812a357a2dfd8e3f68d9a413`  
		Last Modified: Wed, 31 Mar 2021 19:23:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031875ceeaab9b0b96a47b7ed9ec2a0098a9d8662d1c2a57785eb95dbf36d419`  
		Last Modified: Wed, 31 Mar 2021 19:25:23 GMT  
		Size: 102.7 MB (102671786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15870044ac3cd6474d13a6fd94871020ad8801d56fa4387bb9507968da9b093d`  
		Last Modified: Wed, 31 Mar 2021 19:24:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa970c15af3c0912614e0bd697d3329aa1d7f2e98e13f86227bec493367295`  
		Last Modified: Thu, 01 Apr 2021 04:06:04 GMT  
		Size: 7.9 MB (7929419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231389672c1c8c7a9fd39092006eca8983b058e9edc5f0d04bf43bc3f9dea700`  
		Last Modified: Thu, 01 Apr 2021 04:06:02 GMT  
		Size: 1.2 MB (1221595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efaab869ceebc633c179dc051159fb587f7bb30890e765be3f630558cc9933c`  
		Last Modified: Thu, 01 Apr 2021 04:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:673ccce087f4fef545f63f971a0738dbb551fa5872c1742be37a89daded09f29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83363f4d6122099578251753b8d8052a348737a2593393b43b431795fcb64292`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:56:35 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 11:56:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 11:56:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:36:58 GMT
ENV GOLANG_VERSION=1.15.10
# Thu, 01 Apr 2021 12:59:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 01 Apr 2021 12:59:20 GMT
ENV GOPATH=/go
# Thu, 01 Apr 2021 12:59:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 12:59:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 01 Apr 2021 12:59:25 GMT
WORKDIR /go
# Thu, 01 Apr 2021 14:30:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 01 Apr 2021 14:30:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Thu, 01 Apr 2021 14:30:27 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 14:30:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 01 Apr 2021 14:30:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 01 Apr 2021 14:30:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 01 Apr 2021 14:30:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b725919da0175e4c01c41441c29fff6f5ec6c0c4e37417f70120f08f96acfc`  
		Last Modified: Thu, 01 Apr 2021 13:01:16 GMT  
		Size: 280.1 KB (280073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1f51d8714e34d5e746102b7176e77e8142ecf71f4c68d82354285a0bd6d16`  
		Last Modified: Thu, 01 Apr 2021 13:01:15 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d9a84aba5c985724e2f9d0049434534ed654c74b46945f50cc2af08567b9b6`  
		Last Modified: Thu, 01 Apr 2021 13:03:20 GMT  
		Size: 102.5 MB (102462580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc655d7de77ca2ce887998caba1ec52a0bd3f8aa5453bb583ba83449613e96c5`  
		Last Modified: Thu, 01 Apr 2021 13:02:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c177cdf044a6b683b9c1a95121917806970172353334871227cb79e618bc0b1`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 7.1 MB (7145596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac1d6a25abce1b9f81c345e1c2ac0149a173ffdcdca04c5ffd9a450903aa2d2`  
		Last Modified: Thu, 01 Apr 2021 14:31:34 GMT  
		Size: 1.2 MB (1219450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1bc2f6f317df593b6011ce90f58a1234127d7f78cf8121f8972f79d564b69`  
		Last Modified: Thu, 01 Apr 2021 14:31:33 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e8c8a0956ea40a17133ef7055aa4cd1076f944342cddf3665d91c8addbe8effb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114836831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8892c660131d71ee38d69f56f72c5e98aed80471af824bd1ceda7b5a08c2ce4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:51:33 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:57:28 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:00:54 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:01:02 GMT
WORKDIR /go
# Fri, 26 Mar 2021 16:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 16:11:37 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 16:11:38 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 16:11:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 16:11:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 16:11:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 16:11:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f941853f4c183d3b0a653353ba7515088ae2488b01a0ca6bddaa6f1dcc062d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 281.2 KB (281215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4be3bf1d235e013412b55ba1e824da6cfebaf80d284481002d2aa00718563d`  
		Last Modified: Fri, 26 Mar 2021 01:02:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc4f0c823675028e8e8caed39be27c63850615a4394ab508faf5b4ed3a9fc3`  
		Last Modified: Fri, 26 Mar 2021 01:04:37 GMT  
		Size: 102.1 MB (102143643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ce0d84f3cb43a1eb06c18a87965b988275ab2c863043b96032d5d4b94d5db`  
		Last Modified: Fri, 26 Mar 2021 01:04:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6274beb5e6ef4051612c2bcfadde952a3caceb7145e9f6d61ce0b818f2e4f7`  
		Last Modified: Fri, 26 Mar 2021 16:12:33 GMT  
		Size: 8.5 MB (8500012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880cf9840fe472a748b59dbd60483c321b780ac76a1906aafe3c082bfd41496d`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 1.2 MB (1201557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d154a0032206067bed60392933ce1a8bab8e7cd48226b92f0f589d7f1bd746`  
		Last Modified: Fri, 26 Mar 2021 16:12:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b84ae4910f796380e57d7daac89af75d8012094746a88fa467d97bafcdb11fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113985368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b7945ba534d20ab228061857652036740c946d79102221e87b9fb0ea979254`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:50:54 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 26 Mar 2021 00:51:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:51:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 00:58:55 GMT
ENV GOLANG_VERSION=1.15.10
# Fri, 26 Mar 2021 01:01:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 26 Mar 2021 01:01:22 GMT
ENV GOPATH=/go
# Fri, 26 Mar 2021 01:01:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 01:01:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 26 Mar 2021 01:02:00 GMT
WORKDIR /go
# Fri, 26 Mar 2021 05:52:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 26 Mar 2021 05:52:17 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 26 Mar 2021 05:52:23 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:52:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 26 Mar 2021 05:52:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 26 Mar 2021 05:52:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 26 Mar 2021 05:52:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22fc023a51f1560551f97595c0d26436968276b81fd2119cb972238aff23fb6`  
		Last Modified: Fri, 26 Mar 2021 01:06:49 GMT  
		Size: 283.2 KB (283209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b5b049d7abfca6a07577171113a612a55eb6f864651563d204b02fb5c4e60`  
		Last Modified: Fri, 26 Mar 2021 01:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db853427f2ec5049b1f9079b25be4c8117deaa1fcac132410fa8c0b1deb720c8`  
		Last Modified: Fri, 26 Mar 2021 01:12:48 GMT  
		Size: 100.8 MB (100803535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d927b70afd72e9dd133e5d57a45143c8e8ebceefa2dfc3a7fc1bd8e1b9ce83d8`  
		Last Modified: Fri, 26 Mar 2021 01:12:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bf5bc1fa9c61f972e646bacb633a53efd7d173b4d79b2efd32f923d503d50b`  
		Last Modified: Fri, 26 Mar 2021 05:58:21 GMT  
		Size: 8.9 MB (8921440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6874c8aee6bfafc6a12719998f12ce1dcf70d8a61da3dd914f9c791808221`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 1.2 MB (1170494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0826f628855fe686aafb0d3423a1c5258fcb72287998561865187f7e7d4f0`  
		Last Modified: Fri, 26 Mar 2021 05:58:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e7648a8c6fc41f80b2eb8da973742a7485f479cb4f57dcb04d738e8800f5b64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118389839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8b0338c771c7f370f6460e6a444505905acc419685f5c8d35648800e50d8c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:34:37 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 31 Mar 2021 18:34:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:34:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:38:18 GMT
ENV GOLANG_VERSION=1.15.10
# Wed, 31 Mar 2021 18:39:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.10.src.tar.gz'; 	sha256='c1dbca6e0910b41d61a95bf9878f6d6e93d15d884c226b91d9d4b1113c10dd65'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 31 Mar 2021 18:39:46 GMT
ENV GOPATH=/go
# Wed, 31 Mar 2021 18:39:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 31 Mar 2021 18:39:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 31 Mar 2021 18:39:47 GMT
WORKDIR /go
# Wed, 31 Mar 2021 18:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_VERSION=v0.1.8
# Wed, 31 Mar 2021 18:56:15 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 31 Mar 2021 18:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 31 Mar 2021 18:56:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 31 Mar 2021 18:56:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb296d6fc71cd9057e3d03d0ea4ebe30a620f7c6ce57eb78f4c137e77a9a47`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 281.4 KB (281355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783b7db1c405d51f50a261ae252c97941c44ffeb93cb10c2e2bdd458296774a`  
		Last Modified: Wed, 31 Mar 2021 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb58064707977215f9632cdb206eaec9d63534f602e5682c22634dcfbb2cbd5`  
		Last Modified: Wed, 31 Mar 2021 18:42:02 GMT  
		Size: 105.9 MB (105923109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273a64a6b34c09c3baa0d7e2dc15a36980a72e658c1570903625ebac61f7f16`  
		Last Modified: Wed, 31 Mar 2021 18:41:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadae105e5bbdd611f262c9d81668d5b3251f7c246bd9bd444ecd4c88b936326`  
		Last Modified: Wed, 31 Mar 2021 18:57:12 GMT  
		Size: 8.4 MB (8352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7739fc64956105cdc380f5c596d98e8b490d06ca763be1a88849e780ddcc74`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 1.3 MB (1264435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad00fa157eebdd61affab09a5b4d3ba310bf443dca82d624ae508b390df30ea6`  
		Last Modified: Wed, 31 Mar 2021 18:57:11 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:abf97331ba731afdbe77aafef9738f37f5073739ad99cdced920c974c73ca4f4
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
$ docker pull caddy@sha256:629c5800ccf51df482a4e63266e4570de3e573e862d902398b03cbfca2212b4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e073d63a624f18bd8e2f94b9e84715e5a33a817db19afa42afc8ea95e59d568`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:53:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 13:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 13:53:17 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 13:53:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 13:53:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 13:53:21 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 13:53:21 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 13:53:21 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 13:53:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 13:53:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 443
# Thu, 01 Apr 2021 13:53:23 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 13:53:24 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 13:53:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc82ca1670c70e5b605729b271409acba02ca26c3f669bf1d95a067fb853a90`  
		Last Modified: Thu, 01 Apr 2021 13:54:20 GMT  
		Size: 300.0 KB (300021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d66f69260e9358ba74c27e0ed110b9ff7781c5f90d5d01f86d6ef289834382`  
		Last Modified: Thu, 01 Apr 2021 13:54:17 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b38557b1fd80a7712b7263f0896f076afdeb9f25f68a79e288b87490aa3047`  
		Last Modified: Thu, 01 Apr 2021 13:54:19 GMT  
		Size: 11.6 MB (11622380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37d6fba45d5f1633f00b6a9d204abacad2a6918dc355706fe0decc0bc4e565`  
		Last Modified: Thu, 01 Apr 2021 13:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b57cdc61b54865a7ff2ea4ef9d16458537d40e0dc25559d6540111874abbe4ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88293e19906b6b2275ff6e127e29960b1fdf0cf0c4baa4bbce4ea297e90db731`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:36:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 17:36:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 17:36:38 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 17:36:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 17:36:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 17:36:52 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 17:36:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 17:36:55 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 17:36:56 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 17:36:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 17:36:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 17:37:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 17:37:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 17:37:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 17:37:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 17:37:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 17:37:07 GMT
EXPOSE 80
# Wed, 31 Mar 2021 17:37:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 17:37:10 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 17:37:11 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 17:37:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1532456df32c320ccd3c9ff5433c9e44d873ef87a0dc9fc29f9cf256b517eb4`  
		Last Modified: Wed, 31 Mar 2021 17:38:50 GMT  
		Size: 300.1 KB (300103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263f61714ef61a0c59bef8e70bc49a741a357b0a0fc556b44f8344df37ea0f8`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818002dab28746359de43d5a88d06c77cc3a353c838e15c6b6a67d48352cc5c0`  
		Last Modified: Wed, 31 Mar 2021 17:38:54 GMT  
		Size: 10.9 MB (10944835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979a3c808bf5c07c668f5966a15458dbfe9aba5aa7d761e690dd3a5cadf45eb`  
		Last Modified: Wed, 31 Mar 2021 17:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6d510324512c20fc0d40aeb8b6e5b98255c857ad2dee894b6cb6e66f0231cf9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42db38da968682707e6cf0fabb16f93770388907d8a208fca0db74cae3183ba2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:11:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 08:11:47 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 08:11:48 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 08:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 08:11:55 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 08:11:56 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 08:11:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 08:11:58 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 08:11:59 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 08:12:00 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 08:12:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 08:12:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 08:12:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 08:12:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 08:12:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 08:12:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 08:12:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 08:12:09 GMT
EXPOSE 80
# Thu, 01 Apr 2021 08:12:11 GMT
EXPOSE 443
# Thu, 01 Apr 2021 08:12:13 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 08:12:15 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 08:12:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547b5d01ba24abc02b4f05f8134bfb156ce1840f496ed03a1316c882625bd41f`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 299.2 KB (299199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a883a914d37801ae97b0fac82c62e4f70ef4c92fc53417a91a23b2e69d36d9bb`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475143e7b89d1a36700916ec3c8f0caae9b57d5cd9ba187b9f3fd5d9a71eddcf`  
		Last Modified: Thu, 01 Apr 2021 08:13:38 GMT  
		Size: 10.9 MB (10925346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79cdab22a3397c4a98f63a7e96c51881033744b1f198c4984072e7303e9f73`  
		Last Modified: Thu, 01 Apr 2021 08:13:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1c3e6c1b947162789190f9215b56c517caa5c48bd5d09f9753c6ff105ece8ea4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d36a254c95d4ad655ca159d67b79ad8ca4498f82a3c127340a7b5be09e213b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:40:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 12:40:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 12:40:12 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 12:40:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 12:40:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 12:40:35 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 12:40:38 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 12:40:44 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 12:40:49 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 12:40:53 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 12:40:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 12:40:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 12:40:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 12:40:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 12:40:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 12:41:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 12:41:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 12:41:05 GMT
EXPOSE 80
# Thu, 01 Apr 2021 12:41:08 GMT
EXPOSE 443
# Thu, 01 Apr 2021 12:41:12 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 12:41:18 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 12:41:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1fbebcb85e1b4f7457195688308678e46184f78ec8402dcd4eb0992700541`  
		Last Modified: Thu, 01 Apr 2021 12:45:24 GMT  
		Size: 300.3 KB (300333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c34c85964e1be21b929d726522dfd448c029aaf7acd32bf5342ff93070124bd`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c657d5761128c010be222b8ddea92ceba700a3c76afb7704c9d436bbb5582c1`  
		Last Modified: Thu, 01 Apr 2021 12:45:27 GMT  
		Size: 10.6 MB (10598978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90c89f24747de4d19b1c83875e0072662bfe7ce4c5f4e15c551d907b212ebc`  
		Last Modified: Thu, 01 Apr 2021 12:45:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:d8ff14acdf013e9a2df27d95f3326bf7175307a04e9e6f7a40b840bf813898ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63b8a5e4185f59e46edc1e47b15d592327b0c3b8867d3edd3be3a9b3dea5522`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:44 GMT
ADD file:fa3152db8e0ad493ea5fe137f9b6210cabbda6e880fc18f1935b8ef1dae5e5b7 in / 
# Thu, 25 Mar 2021 22:22:50 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:49:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 05:49:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 05:49:51 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 05:50:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 05:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 05:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 05:50:14 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 05:50:24 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 05:50:30 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 05:50:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 05:50:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 05:50:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 05:50:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 05:50:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 05:50:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 05:51:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 05:51:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 05:51:24 GMT
EXPOSE 80
# Fri, 26 Mar 2021 05:51:30 GMT
EXPOSE 443
# Fri, 26 Mar 2021 05:51:35 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 05:51:40 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 05:51:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d9d64eb18374b2d527a335e2362041eba1adef6c7376c1347f45cbd1df5239c1`  
		Last Modified: Thu, 25 Mar 2021 22:24:26 GMT  
		Size: 2.8 MB (2805974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69ab62cc22d6fb5ba7a45731c0b8f378026c7c711d7d48946bfe7c69eae199`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 302.3 KB (302337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9767f7d2aec64fa7c89aa12c9b2b14b03dbe10e20cf53279a88f5009dd2c7841`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502018de7a2dcf0f08830ebcce7c073c9a9db95ecf366d96d44c7a76ba032edc`  
		Last Modified: Fri, 26 Mar 2021 05:58:02 GMT  
		Size: 10.2 MB (10241383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61815e7304b64383c90b6c68c7220f40b74c932f3dd3cfd44b04fed05920aec`  
		Last Modified: Fri, 26 Mar 2021 05:58:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:9d992badb7530225182676af12ae945f5f2de2f5ad7d3946b397892a6de4c123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c8a68869d0806c29e6c2c9c655d3e9085af285c6c24ea651ad3bdffd714e38`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:55:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 31 Mar 2021 18:56:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 31 Mar 2021 18:56:00 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 31 Mar 2021 18:56:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 31 Mar 2021 18:56:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 31 Mar 2021 18:56:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 31 Mar 2021 18:56:05 GMT
VOLUME [/config]
# Wed, 31 Mar 2021 18:56:06 GMT
VOLUME [/data]
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 31 Mar 2021 18:56:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 31 Mar 2021 18:56:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 80
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 443
# Wed, 31 Mar 2021 18:56:08 GMT
EXPOSE 2019
# Wed, 31 Mar 2021 18:56:08 GMT
WORKDIR /srv
# Wed, 31 Mar 2021 18:56:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8eb19b6319d0b09121581759094c3eb58e5574e2063affb6c42c0e1a1937a0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd6e269a873b8a21e2787b0ea05662c0f2676aa9043f52b8884081965be7112`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f6a8a7e19cb11edbda771ce361181202915f4760cdaef5e290b1758cc7b88c`  
		Last Modified: Wed, 31 Mar 2021 18:57:02 GMT  
		Size: 11.3 MB (11272066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec92d2dcab4ee41e4e626d8b360a6feff3822db894894865a36bbe9cfc759df0`  
		Last Modified: Wed, 31 Mar 2021 18:57:00 GMT  
		Size: 154.0 B  
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
