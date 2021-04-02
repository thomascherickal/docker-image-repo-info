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
-	[`caddy:2.4.0-beta.2`](#caddy240-beta2)
-	[`caddy:2.4.0-beta.2-alpine`](#caddy240-beta2-alpine)
-	[`caddy:2.4.0-beta.2-builder`](#caddy240-beta2-builder)
-	[`caddy:2.4.0-beta.2-builder-alpine`](#caddy240-beta2-builder-alpine)
-	[`caddy:2.4.0-beta.2-builder-windowsservercore-1809`](#caddy240-beta2-builder-windowsservercore-1809)
-	[`caddy:2.4.0-beta.2-builder-windowsservercore-ltsc2016`](#caddy240-beta2-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.0-beta.2-windowsservercore`](#caddy240-beta2-windowsservercore)
-	[`caddy:2.4.0-beta.2-windowsservercore-1809`](#caddy240-beta2-windowsservercore-1809)
-	[`caddy:2.4.0-beta.2-windowsservercore-ltsc2016`](#caddy240-beta2-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:f9203a727530897ed215241d9cc3f9ca634445f84eabde0197fd53f5d1e00b0a
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
$ docker pull caddy@sha256:bffc665d927b1ed51d5f36dafc191678472776dea35931198b09deebbe4d31fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f81a6d1059252f032458e7bf5dff42ef2844beec6f1c212b5901fb867fdf0a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:19:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 20:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 20:19:34 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 20:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 20:20:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 20:20:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 20:20:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 20:20:18 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 20:20:23 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 20:20:31 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 20:20:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 20:20:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 20:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 20:21:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 20:21:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 20:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 20:21:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 20:21:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 20:21:27 GMT
EXPOSE 443
# Thu, 01 Apr 2021 20:21:33 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 20:21:42 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 20:21:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc0e09b51c0cca190757d6fc9c2b15a635a361717a65973c8d6edf77918d6d5`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 302.3 KB (302335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091713ba252aea42d1ddb0424ba2c2861b3afd2d0102c5d0a6070bacd31e8b49`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840f6bc70853fb9cc5e9c5752486488368649459a0beaa0684081a5b4a44bd4`  
		Last Modified: Thu, 01 Apr 2021 20:27:42 GMT  
		Size: 10.2 MB (10241392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb03f086aa28c855432404e128ff2009c1198d61578654e584a12062e24953f`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:021184a7ff5b69864870d5968152f6b6235acdfeec77821f1e2be79fd0ea08f4
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
$ docker pull caddy@sha256:bffc665d927b1ed51d5f36dafc191678472776dea35931198b09deebbe4d31fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f81a6d1059252f032458e7bf5dff42ef2844beec6f1c212b5901fb867fdf0a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:19:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 20:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 20:19:34 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 20:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 20:20:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 20:20:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 20:20:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 20:20:18 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 20:20:23 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 20:20:31 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 20:20:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 20:20:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 20:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 20:21:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 20:21:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 20:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 20:21:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 20:21:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 20:21:27 GMT
EXPOSE 443
# Thu, 01 Apr 2021 20:21:33 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 20:21:42 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 20:21:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc0e09b51c0cca190757d6fc9c2b15a635a361717a65973c8d6edf77918d6d5`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 302.3 KB (302335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091713ba252aea42d1ddb0424ba2c2861b3afd2d0102c5d0a6070bacd31e8b49`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840f6bc70853fb9cc5e9c5752486488368649459a0beaa0684081a5b4a44bd4`  
		Last Modified: Thu, 01 Apr 2021 20:27:42 GMT  
		Size: 10.2 MB (10241392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb03f086aa28c855432404e128ff2009c1198d61578654e584a12062e24953f`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:24e707cb4e7f90c12ca1f5fb4c1df08134db8d1ede9b2bce4075f12176f270b2
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
$ docker pull caddy@sha256:ece02ddc55072c0f8170999a314bae216c7a2e9a9b6848e61a6284a9d73f94f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119528273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b85122de32749bb4ce99c4ec210d0b3f4ae7520aeb96d1b3409d7e164a5419`
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
# Fri, 02 Apr 2021 00:26:55 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:28:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:28:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:28:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:28:39 GMT
WORKDIR /go
# Fri, 02 Apr 2021 00:49:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 00:49:44 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 00:49:45 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 00:49:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 00:49:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 00:49:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 00:49:48 GMT
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
	-	`sha256:7fb06cf977208e0278301057f91233255a165debf7803f76081637b1a3fe2df4`  
		Last Modified: Fri, 02 Apr 2021 00:33:59 GMT  
		Size: 106.8 MB (106825493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d4990aca24e7f5bc780b0b6a54b4ffe9309e35aa07fbc5a0a37e0ea3d9f9ba`  
		Last Modified: Fri, 02 Apr 2021 00:33:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82125fdcb93000a2f7bac7bfb8862942871d32af42e10627aacbd1920dccc98b`  
		Last Modified: Fri, 02 Apr 2021 00:50:30 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24a53b2e0122830bff05a8cf66417dca406c3a78c2c50f57ed18b9eabd310c`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 1.3 MB (1311070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8315f3a639f17e3d2f1c8a9375c23b4449414ba0dcfddb8a5b7706e54ad36ef4`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:10d41528f228b48108732d502adc636fca65043411bc0f7290dd76c8edd037cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114712667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:025a88409e4f77fb03240b210876fca131968a56bded41bc910094fed80cf415`
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
# Fri, 02 Apr 2021 01:30:32 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:33:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:33:22 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:33:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:33:34 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:09:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:09:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:09:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:09:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:09:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:09:09 GMT
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
	-	`sha256:4091fa2dc5e0d5be46942830e27d3a5f436a9cb7f46dcc3c113da4dbcbea3040`  
		Last Modified: Fri, 02 Apr 2021 01:39:32 GMT  
		Size: 102.7 MB (102675361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be92ead41aa69a067ce5cb63f8e52a4437d23028ba34a3278d8dd25fefb2fca`  
		Last Modified: Fri, 02 Apr 2021 01:38:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0149c588c89df3be653be7fd1e1adfd8a1294acdf6b72e7389cf0974752985`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 7.9 MB (7929365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e0d86690298b1f2e60ba7793d37b00c6110c464eea7b3f3f55d666976fc4b`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd374a07a01a50e87ff86e4e2aed8910bea99eaa7f85a92e48cddef6ce1695e2`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:055b54c865e8f858fb4592a56a49eccad632fd9d67a45161586e716a68de125c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5ae4a80046d3819c7c459fcdbbb9885b9550347e3ae2d08bf36c6b56ddb901`
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
# Fri, 02 Apr 2021 01:33:58 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:38:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:38:43 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:38:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:38:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:38:54 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:39:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:39:48 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:39:49 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:39:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:39:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:39:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:39:54 GMT
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
	-	`sha256:246e9d6efa3b5ddb94ed08d2c44063063809626f1b8945ab7fd8f608c27b612c`  
		Last Modified: Fri, 02 Apr 2021 01:49:28 GMT  
		Size: 102.5 MB (102462038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185aeca957b64890215aa6243b0ed41133921755346cb5630f47811efe98d924`  
		Last Modified: Fri, 02 Apr 2021 01:48:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561958899ceda559293617ab883e3c7c50ec0d82c29b163b971862b589f19fd7`  
		Last Modified: Fri, 02 Apr 2021 03:40:46 GMT  
		Size: 7.1 MB (7145600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0c3c642c83a6e2e01f091cfa2000f1edd689ea6d1ca5d6fd073c13e795c20`  
		Last Modified: Fri, 02 Apr 2021 03:40:43 GMT  
		Size: 1.2 MB (1219444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d966c9600d6d83b44c77316d87064bcb298ef3c6cc8a488b66eb658be3d31f`  
		Last Modified: Fri, 02 Apr 2021 03:40:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:68996d8d9053274f585d31e72a5606c5b8efc0c22715a722efcb184769dfeb62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114829795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680177f28f49f5cc8e4add6e48c3cf149cc27044bd36825e3ebc2be149c33d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:39:14 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:39:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:04:26 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:07:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:07:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:08:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:08:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:08:57 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:38:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:38:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:38:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:38:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:38:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:38:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:38:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad1fe544e25b6d321ae8fdcd682a086ba01b0cb7a6156e4b56678c814e705a9`  
		Last Modified: Thu, 01 Apr 2021 16:48:38 GMT  
		Size: 281.2 KB (281223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4362df3d97a48df3f56e407e87e3bb4b9ff06e2b28fe3c6b5d9efc43c603c3ea`  
		Last Modified: Thu, 01 Apr 2021 16:48:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf580103e01a743f2033316ab60816b69e6a6d3cc87bd05d4d5e3c01753b59a`  
		Last Modified: Fri, 02 Apr 2021 01:17:28 GMT  
		Size: 102.1 MB (102136450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d59c655ea056d2547111351a9f74cbb1760fd590e7b4d9daf1a3adefabc47`  
		Last Modified: Fri, 02 Apr 2021 01:17:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf4373967e0c510b0e8a50f6a81c276fb4ec40854edffdef61a4101ddcc2d0`  
		Last Modified: Fri, 02 Apr 2021 02:40:20 GMT  
		Size: 8.5 MB (8500007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f4ba979d45ec198f862cb4c75488f29795eeb8706732280704829c8eebb2c`  
		Last Modified: Fri, 02 Apr 2021 02:40:18 GMT  
		Size: 1.2 MB (1201548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ba1a31428dd993c50efd22bf7b473e3505752416376f8d60b61682011823a`  
		Last Modified: Fri, 02 Apr 2021 02:40:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:b4d7764de3f8d29cbb22b2b973802bbf36aa89b6c1e6a11cf6934b2273b80e59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113988669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c777710e48b168e93b792b4171e667a5c16209c668b09dd54d442ad4ef1c55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:33:46 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:33:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:33:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:18:36 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 03:20:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:20:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:20:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:21:02 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:11 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 05:03:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 05:03:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 05:03:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 05:03:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 05:03:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ce9f93b1dd5f42d7663646400f1307cddfad6a5361031e3a1ca8c46d90d2e`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 283.2 KB (283224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb52babc5b3ae7ccfca63bfc4092e7d57cbd51bc203af266e4fcb0169a6107`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91ebeddf57ad09e8e1b3eb1e312be6a4484d88f8f970a7b241d759abe98e5f`  
		Last Modified: Fri, 02 Apr 2021 03:25:31 GMT  
		Size: 100.8 MB (100806744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac05f37b09f2517038025dd2d905a5d3ecbd9af697023fe05bc857ed48b8f455`  
		Last Modified: Fri, 02 Apr 2021 03:25:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e2e6a908474ce0f09d3cc2e30293784024f2a821c330690e753b01155c5346`  
		Last Modified: Fri, 02 Apr 2021 05:04:26 GMT  
		Size: 8.9 MB (8921423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b888e7962a16510b476660b91df0be664af7f16e7eb94288112b51bfd206995`  
		Last Modified: Fri, 02 Apr 2021 05:04:25 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ce4e5965570ab285f5e3be6ab2ca4cd6b618b344303a3e09cbb4c46fb2393f`  
		Last Modified: Fri, 02 Apr 2021 05:04:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:55343bb8a3d3c8060510dda018530e00e140b628136dd4d2e80d5235d9f81310
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118407979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5002b31cde12b4652640e74c39b0c4f6e71cf200aebef971c3dc23634cb9d859`
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
# Fri, 02 Apr 2021 00:47:37 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:48:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:59 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:48:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:59:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:59:07 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:59:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:59:09 GMT
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
	-	`sha256:665e4b76c3c27678347c855f22a12fc05bfe995765d883647a9c2441b9b069d0`  
		Last Modified: Fri, 02 Apr 2021 00:52:06 GMT  
		Size: 105.9 MB (105941238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00e4cb90e6507b991c002adcd7422fee334b80a8f1e5ac783562c6be88675a3`  
		Last Modified: Fri, 02 Apr 2021 00:51:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8845c8ed835494d2be5205c635b53fd5ab4b00d5d26a3334e616c5b014bb0d`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 8.4 MB (8352795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bdec70ad8c727647ea8e85bfee6409d5f5c98958898ba25b0b2fcb779e76fa`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 1.3 MB (1264423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4492bd0a1a8e714b581c18713607112324a6401040484d4ef05de25a16d89`  
		Last Modified: Fri, 02 Apr 2021 02:59:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:89576372020fc2eb4c0a7f3a3e1202a7b5833822dcac78836f6f48dc05cf1b15
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636681347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433619fcb10b7d636ff7d2ab6165f3648a45f1587bf0fc5a17c16bb0b4ea13f9`
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
# Fri, 02 Apr 2021 00:25:42 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:23 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:28:25 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:03:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:03:35 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:03:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:03:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:04:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:04:05 GMT
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
	-	`sha256:ddf005729e9b7c9f2912ff8e30bec3d383755302fe0b20e361d87ed43a703519`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9af25c23d2108f315f14a45d27ecfe24ceb05852132cf721a61ee44495e1a`  
		Last Modified: Fri, 02 Apr 2021 00:44:11 GMT  
		Size: 138.5 MB (138534624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1592b7415bb7c21ec31f9b97bed86b4b01c96621f385d9da5903fa7c320d4e47`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae6b99eb587e6a00f40f4c134c6b7d4b8d1bc9d9d17b14538d30b6c689e5bc2`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d285524127fff971c8f6c086256b3907c8428d162347bcba0f3bcf6d64fa9`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22f3dc30fb1b76d85e47461eb558cc38cd60ccd8d02c6d8bd9aea7cce3e909`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5063c8d06382902b304af0538c9114e087db04e693551e92d15ffd12dcca542`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313a2e87390c3ef15da4fd9f3b978ef539bc6b5bf8d3e54d23f28e4acd386563`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.7 MB (1715051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ed62f1fbb34e8dfbbf3e11e5f7aa91c4e21c7ac1debbbf86e2561d6ecc5ea`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:017255652cc26ea2af428ecc3b6f2222ee64d88cfdf1c34e3522f048aa461ee9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997836720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a9fde1e66982a65a46dea5c07548ac8afcd29b6f304afe23a8ea9bcdcf186f`
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
# Fri, 02 Apr 2021 00:28:41 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:32:35 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:32:37 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:04:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:04:14 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:04:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:04:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:05:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:05:45 GMT
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
	-	`sha256:a055a610a3b2e63b54d561bc3512bd068b4443a7417486b9dc65a4ad292583c7`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c202a262d335726e6d079774ca9e11f52da7326ee18860265595a97527a7b545`  
		Last Modified: Fri, 02 Apr 2021 00:44:55 GMT  
		Size: 144.0 MB (143966864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737da401effa5536406d2508db65af6f54d9be0a3c5f1347ae56dc5ad1b8c1a4`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.6 KB (1579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c52d85af463d5a66468c058122750336a2d002544c19dbaff721875cb8c6c24`  
		Last Modified: Fri, 02 Apr 2021 01:09:48 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f1bf71cbf1adab82ad5a9d8f5b71571306bf6bcf254b686963f2ed7562e7fc`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba22c0fd4b07e8d5ff2ab18028eb3f4d87c20420e43a2afbf78c8da9032399b2`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b238ffe2f30d1bebcac0de5c7d019504926664c08f5730389c7c1e426c12a`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0b00fc7a9cc9546977571c1922da63009fc89865ee5ae6b603cdf38d5b56ad`  
		Last Modified: Fri, 02 Apr 2021 01:09:47 GMT  
		Size: 11.5 MB (11528518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606193453afd7f6b2c5d21cdd640e297c0e3b0514642cc7044ff5a83ef6e66c7`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:7d7b5f18ee38ce53f1af5300bf9d3e4297def83236cbe1769bc50cf631048fa5
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
$ docker pull caddy@sha256:ece02ddc55072c0f8170999a314bae216c7a2e9a9b6848e61a6284a9d73f94f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119528273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b85122de32749bb4ce99c4ec210d0b3f4ae7520aeb96d1b3409d7e164a5419`
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
# Fri, 02 Apr 2021 00:26:55 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:28:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:28:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:28:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:28:39 GMT
WORKDIR /go
# Fri, 02 Apr 2021 00:49:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 00:49:44 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 00:49:45 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 00:49:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 00:49:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 00:49:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 00:49:48 GMT
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
	-	`sha256:7fb06cf977208e0278301057f91233255a165debf7803f76081637b1a3fe2df4`  
		Last Modified: Fri, 02 Apr 2021 00:33:59 GMT  
		Size: 106.8 MB (106825493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d4990aca24e7f5bc780b0b6a54b4ffe9309e35aa07fbc5a0a37e0ea3d9f9ba`  
		Last Modified: Fri, 02 Apr 2021 00:33:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82125fdcb93000a2f7bac7bfb8862942871d32af42e10627aacbd1920dccc98b`  
		Last Modified: Fri, 02 Apr 2021 00:50:30 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24a53b2e0122830bff05a8cf66417dca406c3a78c2c50f57ed18b9eabd310c`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 1.3 MB (1311070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8315f3a639f17e3d2f1c8a9375c23b4449414ba0dcfddb8a5b7706e54ad36ef4`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:10d41528f228b48108732d502adc636fca65043411bc0f7290dd76c8edd037cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114712667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:025a88409e4f77fb03240b210876fca131968a56bded41bc910094fed80cf415`
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
# Fri, 02 Apr 2021 01:30:32 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:33:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:33:22 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:33:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:33:34 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:09:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:09:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:09:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:09:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:09:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:09:09 GMT
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
	-	`sha256:4091fa2dc5e0d5be46942830e27d3a5f436a9cb7f46dcc3c113da4dbcbea3040`  
		Last Modified: Fri, 02 Apr 2021 01:39:32 GMT  
		Size: 102.7 MB (102675361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be92ead41aa69a067ce5cb63f8e52a4437d23028ba34a3278d8dd25fefb2fca`  
		Last Modified: Fri, 02 Apr 2021 01:38:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0149c588c89df3be653be7fd1e1adfd8a1294acdf6b72e7389cf0974752985`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 7.9 MB (7929365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e0d86690298b1f2e60ba7793d37b00c6110c464eea7b3f3f55d666976fc4b`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd374a07a01a50e87ff86e4e2aed8910bea99eaa7f85a92e48cddef6ce1695e2`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:055b54c865e8f858fb4592a56a49eccad632fd9d67a45161586e716a68de125c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5ae4a80046d3819c7c459fcdbbb9885b9550347e3ae2d08bf36c6b56ddb901`
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
# Fri, 02 Apr 2021 01:33:58 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:38:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:38:43 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:38:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:38:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:38:54 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:39:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:39:48 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:39:49 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:39:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:39:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:39:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:39:54 GMT
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
	-	`sha256:246e9d6efa3b5ddb94ed08d2c44063063809626f1b8945ab7fd8f608c27b612c`  
		Last Modified: Fri, 02 Apr 2021 01:49:28 GMT  
		Size: 102.5 MB (102462038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185aeca957b64890215aa6243b0ed41133921755346cb5630f47811efe98d924`  
		Last Modified: Fri, 02 Apr 2021 01:48:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561958899ceda559293617ab883e3c7c50ec0d82c29b163b971862b589f19fd7`  
		Last Modified: Fri, 02 Apr 2021 03:40:46 GMT  
		Size: 7.1 MB (7145600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0c3c642c83a6e2e01f091cfa2000f1edd689ea6d1ca5d6fd073c13e795c20`  
		Last Modified: Fri, 02 Apr 2021 03:40:43 GMT  
		Size: 1.2 MB (1219444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d966c9600d6d83b44c77316d87064bcb298ef3c6cc8a488b66eb658be3d31f`  
		Last Modified: Fri, 02 Apr 2021 03:40:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:68996d8d9053274f585d31e72a5606c5b8efc0c22715a722efcb184769dfeb62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114829795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680177f28f49f5cc8e4add6e48c3cf149cc27044bd36825e3ebc2be149c33d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:39:14 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:39:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:04:26 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:07:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:07:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:08:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:08:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:08:57 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:38:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:38:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:38:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:38:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:38:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:38:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:38:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad1fe544e25b6d321ae8fdcd682a086ba01b0cb7a6156e4b56678c814e705a9`  
		Last Modified: Thu, 01 Apr 2021 16:48:38 GMT  
		Size: 281.2 KB (281223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4362df3d97a48df3f56e407e87e3bb4b9ff06e2b28fe3c6b5d9efc43c603c3ea`  
		Last Modified: Thu, 01 Apr 2021 16:48:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf580103e01a743f2033316ab60816b69e6a6d3cc87bd05d4d5e3c01753b59a`  
		Last Modified: Fri, 02 Apr 2021 01:17:28 GMT  
		Size: 102.1 MB (102136450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d59c655ea056d2547111351a9f74cbb1760fd590e7b4d9daf1a3adefabc47`  
		Last Modified: Fri, 02 Apr 2021 01:17:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf4373967e0c510b0e8a50f6a81c276fb4ec40854edffdef61a4101ddcc2d0`  
		Last Modified: Fri, 02 Apr 2021 02:40:20 GMT  
		Size: 8.5 MB (8500007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f4ba979d45ec198f862cb4c75488f29795eeb8706732280704829c8eebb2c`  
		Last Modified: Fri, 02 Apr 2021 02:40:18 GMT  
		Size: 1.2 MB (1201548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ba1a31428dd993c50efd22bf7b473e3505752416376f8d60b61682011823a`  
		Last Modified: Fri, 02 Apr 2021 02:40:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b4d7764de3f8d29cbb22b2b973802bbf36aa89b6c1e6a11cf6934b2273b80e59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113988669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c777710e48b168e93b792b4171e667a5c16209c668b09dd54d442ad4ef1c55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:33:46 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:33:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:33:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:18:36 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 03:20:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:20:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:20:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:21:02 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:11 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 05:03:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 05:03:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 05:03:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 05:03:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 05:03:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ce9f93b1dd5f42d7663646400f1307cddfad6a5361031e3a1ca8c46d90d2e`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 283.2 KB (283224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb52babc5b3ae7ccfca63bfc4092e7d57cbd51bc203af266e4fcb0169a6107`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91ebeddf57ad09e8e1b3eb1e312be6a4484d88f8f970a7b241d759abe98e5f`  
		Last Modified: Fri, 02 Apr 2021 03:25:31 GMT  
		Size: 100.8 MB (100806744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac05f37b09f2517038025dd2d905a5d3ecbd9af697023fe05bc857ed48b8f455`  
		Last Modified: Fri, 02 Apr 2021 03:25:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e2e6a908474ce0f09d3cc2e30293784024f2a821c330690e753b01155c5346`  
		Last Modified: Fri, 02 Apr 2021 05:04:26 GMT  
		Size: 8.9 MB (8921423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b888e7962a16510b476660b91df0be664af7f16e7eb94288112b51bfd206995`  
		Last Modified: Fri, 02 Apr 2021 05:04:25 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ce4e5965570ab285f5e3be6ab2ca4cd6b618b344303a3e09cbb4c46fb2393f`  
		Last Modified: Fri, 02 Apr 2021 05:04:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:55343bb8a3d3c8060510dda018530e00e140b628136dd4d2e80d5235d9f81310
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118407979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5002b31cde12b4652640e74c39b0c4f6e71cf200aebef971c3dc23634cb9d859`
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
# Fri, 02 Apr 2021 00:47:37 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:48:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:59 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:48:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:59:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:59:07 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:59:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:59:09 GMT
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
	-	`sha256:665e4b76c3c27678347c855f22a12fc05bfe995765d883647a9c2441b9b069d0`  
		Last Modified: Fri, 02 Apr 2021 00:52:06 GMT  
		Size: 105.9 MB (105941238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00e4cb90e6507b991c002adcd7422fee334b80a8f1e5ac783562c6be88675a3`  
		Last Modified: Fri, 02 Apr 2021 00:51:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8845c8ed835494d2be5205c635b53fd5ab4b00d5d26a3334e616c5b014bb0d`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 8.4 MB (8352795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bdec70ad8c727647ea8e85bfee6409d5f5c98958898ba25b0b2fcb779e76fa`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 1.3 MB (1264423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4492bd0a1a8e714b581c18713607112324a6401040484d4ef05de25a16d89`  
		Last Modified: Fri, 02 Apr 2021 02:59:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:0c67e10ec967bbb5febbb8307b0e4a234df003c616262fde938f75631cacd2e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:89576372020fc2eb4c0a7f3a3e1202a7b5833822dcac78836f6f48dc05cf1b15
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636681347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433619fcb10b7d636ff7d2ab6165f3648a45f1587bf0fc5a17c16bb0b4ea13f9`
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
# Fri, 02 Apr 2021 00:25:42 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:23 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:28:25 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:03:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:03:35 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:03:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:03:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:04:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:04:05 GMT
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
	-	`sha256:ddf005729e9b7c9f2912ff8e30bec3d383755302fe0b20e361d87ed43a703519`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9af25c23d2108f315f14a45d27ecfe24ceb05852132cf721a61ee44495e1a`  
		Last Modified: Fri, 02 Apr 2021 00:44:11 GMT  
		Size: 138.5 MB (138534624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1592b7415bb7c21ec31f9b97bed86b4b01c96621f385d9da5903fa7c320d4e47`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae6b99eb587e6a00f40f4c134c6b7d4b8d1bc9d9d17b14538d30b6c689e5bc2`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d285524127fff971c8f6c086256b3907c8428d162347bcba0f3bcf6d64fa9`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22f3dc30fb1b76d85e47461eb558cc38cd60ccd8d02c6d8bd9aea7cce3e909`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5063c8d06382902b304af0538c9114e087db04e693551e92d15ffd12dcca542`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313a2e87390c3ef15da4fd9f3b978ef539bc6b5bf8d3e54d23f28e4acd386563`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.7 MB (1715051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ed62f1fbb34e8dfbbf3e11e5f7aa91c4e21c7ac1debbbf86e2561d6ecc5ea`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:707fee0b94dcb8bb07e1cc0f86e10c540509ee572b69240bc0556cfafa586cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:017255652cc26ea2af428ecc3b6f2222ee64d88cfdf1c34e3522f048aa461ee9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997836720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a9fde1e66982a65a46dea5c07548ac8afcd29b6f304afe23a8ea9bcdcf186f`
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
# Fri, 02 Apr 2021 00:28:41 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:32:35 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:32:37 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:04:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:04:14 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:04:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:04:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:05:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:05:45 GMT
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
	-	`sha256:a055a610a3b2e63b54d561bc3512bd068b4443a7417486b9dc65a4ad292583c7`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c202a262d335726e6d079774ca9e11f52da7326ee18860265595a97527a7b545`  
		Last Modified: Fri, 02 Apr 2021 00:44:55 GMT  
		Size: 144.0 MB (143966864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737da401effa5536406d2508db65af6f54d9be0a3c5f1347ae56dc5ad1b8c1a4`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.6 KB (1579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c52d85af463d5a66468c058122750336a2d002544c19dbaff721875cb8c6c24`  
		Last Modified: Fri, 02 Apr 2021 01:09:48 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f1bf71cbf1adab82ad5a9d8f5b71571306bf6bcf254b686963f2ed7562e7fc`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba22c0fd4b07e8d5ff2ab18028eb3f4d87c20420e43a2afbf78c8da9032399b2`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b238ffe2f30d1bebcac0de5c7d019504926664c08f5730389c7c1e426c12a`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0b00fc7a9cc9546977571c1922da63009fc89865ee5ae6b603cdf38d5b56ad`  
		Last Modified: Fri, 02 Apr 2021 01:09:47 GMT  
		Size: 11.5 MB (11528518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606193453afd7f6b2c5d21cdd640e297c0e3b0514642cc7044ff5a83ef6e66c7`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1309 bytes)  
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
$ docker pull caddy@sha256:f9203a727530897ed215241d9cc3f9ca634445f84eabde0197fd53f5d1e00b0a
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
$ docker pull caddy@sha256:bffc665d927b1ed51d5f36dafc191678472776dea35931198b09deebbe4d31fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f81a6d1059252f032458e7bf5dff42ef2844beec6f1c212b5901fb867fdf0a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:19:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 20:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 20:19:34 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 20:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 20:20:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 20:20:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 20:20:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 20:20:18 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 20:20:23 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 20:20:31 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 20:20:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 20:20:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 20:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 20:21:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 20:21:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 20:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 20:21:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 20:21:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 20:21:27 GMT
EXPOSE 443
# Thu, 01 Apr 2021 20:21:33 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 20:21:42 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 20:21:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc0e09b51c0cca190757d6fc9c2b15a635a361717a65973c8d6edf77918d6d5`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 302.3 KB (302335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091713ba252aea42d1ddb0424ba2c2861b3afd2d0102c5d0a6070bacd31e8b49`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840f6bc70853fb9cc5e9c5752486488368649459a0beaa0684081a5b4a44bd4`  
		Last Modified: Thu, 01 Apr 2021 20:27:42 GMT  
		Size: 10.2 MB (10241392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb03f086aa28c855432404e128ff2009c1198d61578654e584a12062e24953f`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:021184a7ff5b69864870d5968152f6b6235acdfeec77821f1e2be79fd0ea08f4
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
$ docker pull caddy@sha256:bffc665d927b1ed51d5f36dafc191678472776dea35931198b09deebbe4d31fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f81a6d1059252f032458e7bf5dff42ef2844beec6f1c212b5901fb867fdf0a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:19:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 20:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 20:19:34 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 20:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 20:20:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 20:20:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 20:20:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 20:20:18 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 20:20:23 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 20:20:31 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 20:20:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 20:20:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 20:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 20:21:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 20:21:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 20:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 20:21:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 20:21:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 20:21:27 GMT
EXPOSE 443
# Thu, 01 Apr 2021 20:21:33 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 20:21:42 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 20:21:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc0e09b51c0cca190757d6fc9c2b15a635a361717a65973c8d6edf77918d6d5`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 302.3 KB (302335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091713ba252aea42d1ddb0424ba2c2861b3afd2d0102c5d0a6070bacd31e8b49`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840f6bc70853fb9cc5e9c5752486488368649459a0beaa0684081a5b4a44bd4`  
		Last Modified: Thu, 01 Apr 2021 20:27:42 GMT  
		Size: 10.2 MB (10241392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb03f086aa28c855432404e128ff2009c1198d61578654e584a12062e24953f`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:24e707cb4e7f90c12ca1f5fb4c1df08134db8d1ede9b2bce4075f12176f270b2
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
$ docker pull caddy@sha256:ece02ddc55072c0f8170999a314bae216c7a2e9a9b6848e61a6284a9d73f94f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119528273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b85122de32749bb4ce99c4ec210d0b3f4ae7520aeb96d1b3409d7e164a5419`
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
# Fri, 02 Apr 2021 00:26:55 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:28:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:28:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:28:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:28:39 GMT
WORKDIR /go
# Fri, 02 Apr 2021 00:49:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 00:49:44 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 00:49:45 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 00:49:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 00:49:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 00:49:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 00:49:48 GMT
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
	-	`sha256:7fb06cf977208e0278301057f91233255a165debf7803f76081637b1a3fe2df4`  
		Last Modified: Fri, 02 Apr 2021 00:33:59 GMT  
		Size: 106.8 MB (106825493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d4990aca24e7f5bc780b0b6a54b4ffe9309e35aa07fbc5a0a37e0ea3d9f9ba`  
		Last Modified: Fri, 02 Apr 2021 00:33:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82125fdcb93000a2f7bac7bfb8862942871d32af42e10627aacbd1920dccc98b`  
		Last Modified: Fri, 02 Apr 2021 00:50:30 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24a53b2e0122830bff05a8cf66417dca406c3a78c2c50f57ed18b9eabd310c`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 1.3 MB (1311070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8315f3a639f17e3d2f1c8a9375c23b4449414ba0dcfddb8a5b7706e54ad36ef4`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:10d41528f228b48108732d502adc636fca65043411bc0f7290dd76c8edd037cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114712667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:025a88409e4f77fb03240b210876fca131968a56bded41bc910094fed80cf415`
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
# Fri, 02 Apr 2021 01:30:32 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:33:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:33:22 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:33:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:33:34 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:09:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:09:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:09:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:09:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:09:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:09:09 GMT
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
	-	`sha256:4091fa2dc5e0d5be46942830e27d3a5f436a9cb7f46dcc3c113da4dbcbea3040`  
		Last Modified: Fri, 02 Apr 2021 01:39:32 GMT  
		Size: 102.7 MB (102675361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be92ead41aa69a067ce5cb63f8e52a4437d23028ba34a3278d8dd25fefb2fca`  
		Last Modified: Fri, 02 Apr 2021 01:38:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0149c588c89df3be653be7fd1e1adfd8a1294acdf6b72e7389cf0974752985`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 7.9 MB (7929365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e0d86690298b1f2e60ba7793d37b00c6110c464eea7b3f3f55d666976fc4b`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd374a07a01a50e87ff86e4e2aed8910bea99eaa7f85a92e48cddef6ce1695e2`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:055b54c865e8f858fb4592a56a49eccad632fd9d67a45161586e716a68de125c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5ae4a80046d3819c7c459fcdbbb9885b9550347e3ae2d08bf36c6b56ddb901`
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
# Fri, 02 Apr 2021 01:33:58 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:38:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:38:43 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:38:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:38:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:38:54 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:39:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:39:48 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:39:49 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:39:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:39:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:39:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:39:54 GMT
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
	-	`sha256:246e9d6efa3b5ddb94ed08d2c44063063809626f1b8945ab7fd8f608c27b612c`  
		Last Modified: Fri, 02 Apr 2021 01:49:28 GMT  
		Size: 102.5 MB (102462038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185aeca957b64890215aa6243b0ed41133921755346cb5630f47811efe98d924`  
		Last Modified: Fri, 02 Apr 2021 01:48:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561958899ceda559293617ab883e3c7c50ec0d82c29b163b971862b589f19fd7`  
		Last Modified: Fri, 02 Apr 2021 03:40:46 GMT  
		Size: 7.1 MB (7145600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0c3c642c83a6e2e01f091cfa2000f1edd689ea6d1ca5d6fd073c13e795c20`  
		Last Modified: Fri, 02 Apr 2021 03:40:43 GMT  
		Size: 1.2 MB (1219444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d966c9600d6d83b44c77316d87064bcb298ef3c6cc8a488b66eb658be3d31f`  
		Last Modified: Fri, 02 Apr 2021 03:40:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:68996d8d9053274f585d31e72a5606c5b8efc0c22715a722efcb184769dfeb62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114829795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680177f28f49f5cc8e4add6e48c3cf149cc27044bd36825e3ebc2be149c33d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:39:14 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:39:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:04:26 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:07:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:07:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:08:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:08:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:08:57 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:38:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:38:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:38:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:38:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:38:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:38:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:38:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad1fe544e25b6d321ae8fdcd682a086ba01b0cb7a6156e4b56678c814e705a9`  
		Last Modified: Thu, 01 Apr 2021 16:48:38 GMT  
		Size: 281.2 KB (281223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4362df3d97a48df3f56e407e87e3bb4b9ff06e2b28fe3c6b5d9efc43c603c3ea`  
		Last Modified: Thu, 01 Apr 2021 16:48:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf580103e01a743f2033316ab60816b69e6a6d3cc87bd05d4d5e3c01753b59a`  
		Last Modified: Fri, 02 Apr 2021 01:17:28 GMT  
		Size: 102.1 MB (102136450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d59c655ea056d2547111351a9f74cbb1760fd590e7b4d9daf1a3adefabc47`  
		Last Modified: Fri, 02 Apr 2021 01:17:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf4373967e0c510b0e8a50f6a81c276fb4ec40854edffdef61a4101ddcc2d0`  
		Last Modified: Fri, 02 Apr 2021 02:40:20 GMT  
		Size: 8.5 MB (8500007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f4ba979d45ec198f862cb4c75488f29795eeb8706732280704829c8eebb2c`  
		Last Modified: Fri, 02 Apr 2021 02:40:18 GMT  
		Size: 1.2 MB (1201548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ba1a31428dd993c50efd22bf7b473e3505752416376f8d60b61682011823a`  
		Last Modified: Fri, 02 Apr 2021 02:40:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:b4d7764de3f8d29cbb22b2b973802bbf36aa89b6c1e6a11cf6934b2273b80e59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113988669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c777710e48b168e93b792b4171e667a5c16209c668b09dd54d442ad4ef1c55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:33:46 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:33:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:33:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:18:36 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 03:20:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:20:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:20:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:21:02 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:11 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 05:03:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 05:03:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 05:03:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 05:03:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 05:03:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ce9f93b1dd5f42d7663646400f1307cddfad6a5361031e3a1ca8c46d90d2e`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 283.2 KB (283224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb52babc5b3ae7ccfca63bfc4092e7d57cbd51bc203af266e4fcb0169a6107`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91ebeddf57ad09e8e1b3eb1e312be6a4484d88f8f970a7b241d759abe98e5f`  
		Last Modified: Fri, 02 Apr 2021 03:25:31 GMT  
		Size: 100.8 MB (100806744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac05f37b09f2517038025dd2d905a5d3ecbd9af697023fe05bc857ed48b8f455`  
		Last Modified: Fri, 02 Apr 2021 03:25:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e2e6a908474ce0f09d3cc2e30293784024f2a821c330690e753b01155c5346`  
		Last Modified: Fri, 02 Apr 2021 05:04:26 GMT  
		Size: 8.9 MB (8921423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b888e7962a16510b476660b91df0be664af7f16e7eb94288112b51bfd206995`  
		Last Modified: Fri, 02 Apr 2021 05:04:25 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ce4e5965570ab285f5e3be6ab2ca4cd6b618b344303a3e09cbb4c46fb2393f`  
		Last Modified: Fri, 02 Apr 2021 05:04:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:55343bb8a3d3c8060510dda018530e00e140b628136dd4d2e80d5235d9f81310
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118407979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5002b31cde12b4652640e74c39b0c4f6e71cf200aebef971c3dc23634cb9d859`
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
# Fri, 02 Apr 2021 00:47:37 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:48:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:59 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:48:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:59:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:59:07 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:59:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:59:09 GMT
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
	-	`sha256:665e4b76c3c27678347c855f22a12fc05bfe995765d883647a9c2441b9b069d0`  
		Last Modified: Fri, 02 Apr 2021 00:52:06 GMT  
		Size: 105.9 MB (105941238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00e4cb90e6507b991c002adcd7422fee334b80a8f1e5ac783562c6be88675a3`  
		Last Modified: Fri, 02 Apr 2021 00:51:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8845c8ed835494d2be5205c635b53fd5ab4b00d5d26a3334e616c5b014bb0d`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 8.4 MB (8352795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bdec70ad8c727647ea8e85bfee6409d5f5c98958898ba25b0b2fcb779e76fa`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 1.3 MB (1264423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4492bd0a1a8e714b581c18713607112324a6401040484d4ef05de25a16d89`  
		Last Modified: Fri, 02 Apr 2021 02:59:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:89576372020fc2eb4c0a7f3a3e1202a7b5833822dcac78836f6f48dc05cf1b15
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636681347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433619fcb10b7d636ff7d2ab6165f3648a45f1587bf0fc5a17c16bb0b4ea13f9`
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
# Fri, 02 Apr 2021 00:25:42 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:23 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:28:25 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:03:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:03:35 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:03:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:03:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:04:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:04:05 GMT
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
	-	`sha256:ddf005729e9b7c9f2912ff8e30bec3d383755302fe0b20e361d87ed43a703519`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9af25c23d2108f315f14a45d27ecfe24ceb05852132cf721a61ee44495e1a`  
		Last Modified: Fri, 02 Apr 2021 00:44:11 GMT  
		Size: 138.5 MB (138534624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1592b7415bb7c21ec31f9b97bed86b4b01c96621f385d9da5903fa7c320d4e47`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae6b99eb587e6a00f40f4c134c6b7d4b8d1bc9d9d17b14538d30b6c689e5bc2`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d285524127fff971c8f6c086256b3907c8428d162347bcba0f3bcf6d64fa9`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22f3dc30fb1b76d85e47461eb558cc38cd60ccd8d02c6d8bd9aea7cce3e909`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5063c8d06382902b304af0538c9114e087db04e693551e92d15ffd12dcca542`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313a2e87390c3ef15da4fd9f3b978ef539bc6b5bf8d3e54d23f28e4acd386563`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.7 MB (1715051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ed62f1fbb34e8dfbbf3e11e5f7aa91c4e21c7ac1debbbf86e2561d6ecc5ea`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:017255652cc26ea2af428ecc3b6f2222ee64d88cfdf1c34e3522f048aa461ee9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997836720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a9fde1e66982a65a46dea5c07548ac8afcd29b6f304afe23a8ea9bcdcf186f`
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
# Fri, 02 Apr 2021 00:28:41 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:32:35 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:32:37 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:04:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:04:14 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:04:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:04:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:05:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:05:45 GMT
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
	-	`sha256:a055a610a3b2e63b54d561bc3512bd068b4443a7417486b9dc65a4ad292583c7`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c202a262d335726e6d079774ca9e11f52da7326ee18860265595a97527a7b545`  
		Last Modified: Fri, 02 Apr 2021 00:44:55 GMT  
		Size: 144.0 MB (143966864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737da401effa5536406d2508db65af6f54d9be0a3c5f1347ae56dc5ad1b8c1a4`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.6 KB (1579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c52d85af463d5a66468c058122750336a2d002544c19dbaff721875cb8c6c24`  
		Last Modified: Fri, 02 Apr 2021 01:09:48 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f1bf71cbf1adab82ad5a9d8f5b71571306bf6bcf254b686963f2ed7562e7fc`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba22c0fd4b07e8d5ff2ab18028eb3f4d87c20420e43a2afbf78c8da9032399b2`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b238ffe2f30d1bebcac0de5c7d019504926664c08f5730389c7c1e426c12a`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0b00fc7a9cc9546977571c1922da63009fc89865ee5ae6b603cdf38d5b56ad`  
		Last Modified: Fri, 02 Apr 2021 01:09:47 GMT  
		Size: 11.5 MB (11528518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606193453afd7f6b2c5d21cdd640e297c0e3b0514642cc7044ff5a83ef6e66c7`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-alpine`

```console
$ docker pull caddy@sha256:7d7b5f18ee38ce53f1af5300bf9d3e4297def83236cbe1769bc50cf631048fa5
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
$ docker pull caddy@sha256:ece02ddc55072c0f8170999a314bae216c7a2e9a9b6848e61a6284a9d73f94f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119528273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b85122de32749bb4ce99c4ec210d0b3f4ae7520aeb96d1b3409d7e164a5419`
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
# Fri, 02 Apr 2021 00:26:55 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:28:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:28:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:28:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:28:39 GMT
WORKDIR /go
# Fri, 02 Apr 2021 00:49:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 00:49:44 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 00:49:45 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 00:49:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 00:49:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 00:49:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 00:49:48 GMT
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
	-	`sha256:7fb06cf977208e0278301057f91233255a165debf7803f76081637b1a3fe2df4`  
		Last Modified: Fri, 02 Apr 2021 00:33:59 GMT  
		Size: 106.8 MB (106825493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d4990aca24e7f5bc780b0b6a54b4ffe9309e35aa07fbc5a0a37e0ea3d9f9ba`  
		Last Modified: Fri, 02 Apr 2021 00:33:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82125fdcb93000a2f7bac7bfb8862942871d32af42e10627aacbd1920dccc98b`  
		Last Modified: Fri, 02 Apr 2021 00:50:30 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24a53b2e0122830bff05a8cf66417dca406c3a78c2c50f57ed18b9eabd310c`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 1.3 MB (1311070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8315f3a639f17e3d2f1c8a9375c23b4449414ba0dcfddb8a5b7706e54ad36ef4`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:10d41528f228b48108732d502adc636fca65043411bc0f7290dd76c8edd037cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114712667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:025a88409e4f77fb03240b210876fca131968a56bded41bc910094fed80cf415`
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
# Fri, 02 Apr 2021 01:30:32 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:33:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:33:22 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:33:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:33:34 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:09:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:09:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:09:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:09:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:09:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:09:09 GMT
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
	-	`sha256:4091fa2dc5e0d5be46942830e27d3a5f436a9cb7f46dcc3c113da4dbcbea3040`  
		Last Modified: Fri, 02 Apr 2021 01:39:32 GMT  
		Size: 102.7 MB (102675361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be92ead41aa69a067ce5cb63f8e52a4437d23028ba34a3278d8dd25fefb2fca`  
		Last Modified: Fri, 02 Apr 2021 01:38:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0149c588c89df3be653be7fd1e1adfd8a1294acdf6b72e7389cf0974752985`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 7.9 MB (7929365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e0d86690298b1f2e60ba7793d37b00c6110c464eea7b3f3f55d666976fc4b`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd374a07a01a50e87ff86e4e2aed8910bea99eaa7f85a92e48cddef6ce1695e2`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:055b54c865e8f858fb4592a56a49eccad632fd9d67a45161586e716a68de125c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5ae4a80046d3819c7c459fcdbbb9885b9550347e3ae2d08bf36c6b56ddb901`
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
# Fri, 02 Apr 2021 01:33:58 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:38:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:38:43 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:38:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:38:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:38:54 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:39:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:39:48 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:39:49 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:39:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:39:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:39:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:39:54 GMT
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
	-	`sha256:246e9d6efa3b5ddb94ed08d2c44063063809626f1b8945ab7fd8f608c27b612c`  
		Last Modified: Fri, 02 Apr 2021 01:49:28 GMT  
		Size: 102.5 MB (102462038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185aeca957b64890215aa6243b0ed41133921755346cb5630f47811efe98d924`  
		Last Modified: Fri, 02 Apr 2021 01:48:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561958899ceda559293617ab883e3c7c50ec0d82c29b163b971862b589f19fd7`  
		Last Modified: Fri, 02 Apr 2021 03:40:46 GMT  
		Size: 7.1 MB (7145600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0c3c642c83a6e2e01f091cfa2000f1edd689ea6d1ca5d6fd073c13e795c20`  
		Last Modified: Fri, 02 Apr 2021 03:40:43 GMT  
		Size: 1.2 MB (1219444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d966c9600d6d83b44c77316d87064bcb298ef3c6cc8a488b66eb658be3d31f`  
		Last Modified: Fri, 02 Apr 2021 03:40:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:68996d8d9053274f585d31e72a5606c5b8efc0c22715a722efcb184769dfeb62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114829795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680177f28f49f5cc8e4add6e48c3cf149cc27044bd36825e3ebc2be149c33d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:39:14 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:39:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:04:26 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:07:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:07:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:08:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:08:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:08:57 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:38:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:38:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:38:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:38:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:38:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:38:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:38:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad1fe544e25b6d321ae8fdcd682a086ba01b0cb7a6156e4b56678c814e705a9`  
		Last Modified: Thu, 01 Apr 2021 16:48:38 GMT  
		Size: 281.2 KB (281223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4362df3d97a48df3f56e407e87e3bb4b9ff06e2b28fe3c6b5d9efc43c603c3ea`  
		Last Modified: Thu, 01 Apr 2021 16:48:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf580103e01a743f2033316ab60816b69e6a6d3cc87bd05d4d5e3c01753b59a`  
		Last Modified: Fri, 02 Apr 2021 01:17:28 GMT  
		Size: 102.1 MB (102136450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d59c655ea056d2547111351a9f74cbb1760fd590e7b4d9daf1a3adefabc47`  
		Last Modified: Fri, 02 Apr 2021 01:17:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf4373967e0c510b0e8a50f6a81c276fb4ec40854edffdef61a4101ddcc2d0`  
		Last Modified: Fri, 02 Apr 2021 02:40:20 GMT  
		Size: 8.5 MB (8500007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f4ba979d45ec198f862cb4c75488f29795eeb8706732280704829c8eebb2c`  
		Last Modified: Fri, 02 Apr 2021 02:40:18 GMT  
		Size: 1.2 MB (1201548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ba1a31428dd993c50efd22bf7b473e3505752416376f8d60b61682011823a`  
		Last Modified: Fri, 02 Apr 2021 02:40:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b4d7764de3f8d29cbb22b2b973802bbf36aa89b6c1e6a11cf6934b2273b80e59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113988669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c777710e48b168e93b792b4171e667a5c16209c668b09dd54d442ad4ef1c55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:33:46 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:33:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:33:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:18:36 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 03:20:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:20:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:20:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:21:02 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:11 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 05:03:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 05:03:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 05:03:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 05:03:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 05:03:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ce9f93b1dd5f42d7663646400f1307cddfad6a5361031e3a1ca8c46d90d2e`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 283.2 KB (283224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb52babc5b3ae7ccfca63bfc4092e7d57cbd51bc203af266e4fcb0169a6107`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91ebeddf57ad09e8e1b3eb1e312be6a4484d88f8f970a7b241d759abe98e5f`  
		Last Modified: Fri, 02 Apr 2021 03:25:31 GMT  
		Size: 100.8 MB (100806744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac05f37b09f2517038025dd2d905a5d3ecbd9af697023fe05bc857ed48b8f455`  
		Last Modified: Fri, 02 Apr 2021 03:25:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e2e6a908474ce0f09d3cc2e30293784024f2a821c330690e753b01155c5346`  
		Last Modified: Fri, 02 Apr 2021 05:04:26 GMT  
		Size: 8.9 MB (8921423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b888e7962a16510b476660b91df0be664af7f16e7eb94288112b51bfd206995`  
		Last Modified: Fri, 02 Apr 2021 05:04:25 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ce4e5965570ab285f5e3be6ab2ca4cd6b618b344303a3e09cbb4c46fb2393f`  
		Last Modified: Fri, 02 Apr 2021 05:04:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:55343bb8a3d3c8060510dda018530e00e140b628136dd4d2e80d5235d9f81310
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118407979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5002b31cde12b4652640e74c39b0c4f6e71cf200aebef971c3dc23634cb9d859`
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
# Fri, 02 Apr 2021 00:47:37 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:48:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:59 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:48:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:59:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:59:07 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:59:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:59:09 GMT
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
	-	`sha256:665e4b76c3c27678347c855f22a12fc05bfe995765d883647a9c2441b9b069d0`  
		Last Modified: Fri, 02 Apr 2021 00:52:06 GMT  
		Size: 105.9 MB (105941238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00e4cb90e6507b991c002adcd7422fee334b80a8f1e5ac783562c6be88675a3`  
		Last Modified: Fri, 02 Apr 2021 00:51:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8845c8ed835494d2be5205c635b53fd5ab4b00d5d26a3334e616c5b014bb0d`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 8.4 MB (8352795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bdec70ad8c727647ea8e85bfee6409d5f5c98958898ba25b0b2fcb779e76fa`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 1.3 MB (1264423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4492bd0a1a8e714b581c18713607112324a6401040484d4ef05de25a16d89`  
		Last Modified: Fri, 02 Apr 2021 02:59:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:0c67e10ec967bbb5febbb8307b0e4a234df003c616262fde938f75631cacd2e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:89576372020fc2eb4c0a7f3a3e1202a7b5833822dcac78836f6f48dc05cf1b15
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636681347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433619fcb10b7d636ff7d2ab6165f3648a45f1587bf0fc5a17c16bb0b4ea13f9`
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
# Fri, 02 Apr 2021 00:25:42 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:23 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:28:25 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:03:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:03:35 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:03:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:03:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:04:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:04:05 GMT
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
	-	`sha256:ddf005729e9b7c9f2912ff8e30bec3d383755302fe0b20e361d87ed43a703519`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9af25c23d2108f315f14a45d27ecfe24ceb05852132cf721a61ee44495e1a`  
		Last Modified: Fri, 02 Apr 2021 00:44:11 GMT  
		Size: 138.5 MB (138534624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1592b7415bb7c21ec31f9b97bed86b4b01c96621f385d9da5903fa7c320d4e47`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae6b99eb587e6a00f40f4c134c6b7d4b8d1bc9d9d17b14538d30b6c689e5bc2`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d285524127fff971c8f6c086256b3907c8428d162347bcba0f3bcf6d64fa9`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22f3dc30fb1b76d85e47461eb558cc38cd60ccd8d02c6d8bd9aea7cce3e909`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5063c8d06382902b304af0538c9114e087db04e693551e92d15ffd12dcca542`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313a2e87390c3ef15da4fd9f3b978ef539bc6b5bf8d3e54d23f28e4acd386563`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.7 MB (1715051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ed62f1fbb34e8dfbbf3e11e5f7aa91c4e21c7ac1debbbf86e2561d6ecc5ea`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:707fee0b94dcb8bb07e1cc0f86e10c540509ee572b69240bc0556cfafa586cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:017255652cc26ea2af428ecc3b6f2222ee64d88cfdf1c34e3522f048aa461ee9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997836720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a9fde1e66982a65a46dea5c07548ac8afcd29b6f304afe23a8ea9bcdcf186f`
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
# Fri, 02 Apr 2021 00:28:41 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:32:35 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:32:37 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:04:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:04:14 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:04:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:04:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:05:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:05:45 GMT
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
	-	`sha256:a055a610a3b2e63b54d561bc3512bd068b4443a7417486b9dc65a4ad292583c7`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c202a262d335726e6d079774ca9e11f52da7326ee18860265595a97527a7b545`  
		Last Modified: Fri, 02 Apr 2021 00:44:55 GMT  
		Size: 144.0 MB (143966864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737da401effa5536406d2508db65af6f54d9be0a3c5f1347ae56dc5ad1b8c1a4`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.6 KB (1579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c52d85af463d5a66468c058122750336a2d002544c19dbaff721875cb8c6c24`  
		Last Modified: Fri, 02 Apr 2021 01:09:48 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f1bf71cbf1adab82ad5a9d8f5b71571306bf6bcf254b686963f2ed7562e7fc`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba22c0fd4b07e8d5ff2ab18028eb3f4d87c20420e43a2afbf78c8da9032399b2`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b238ffe2f30d1bebcac0de5c7d019504926664c08f5730389c7c1e426c12a`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0b00fc7a9cc9546977571c1922da63009fc89865ee5ae6b603cdf38d5b56ad`  
		Last Modified: Fri, 02 Apr 2021 01:09:47 GMT  
		Size: 11.5 MB (11528518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606193453afd7f6b2c5d21cdd640e297c0e3b0514642cc7044ff5a83ef6e66c7`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1309 bytes)  
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

## `caddy:2.4.0-beta.2`

```console
$ docker pull caddy@sha256:23c073062ccee33cd49f24ea2b9c9932ea8a002aa8e726d81ef152c47be41422
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

### `caddy:2.4.0-beta.2` - linux; amd64

```console
$ docker pull caddy@sha256:fa50efe45a26d4e0d4ee53589eefc94adc848e23599088e3a23fa8a46e37b0ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14525653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c90ba77981732d04067f9d48287ef8cabe5c59a33c4561d4668fbe43695bc0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Fri, 02 Apr 2021 18:19:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:19:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:19:34 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:19:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:19:38 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:19:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:19:38 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:19:38 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:19:38 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:19:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:19:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:19:40 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:19:40 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:19:40 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:19:41 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:19:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212f6a1c9e4977bde3df77a8a6c46bf7757d599f51a15eb01c63bd2be543cb40`  
		Last Modified: Fri, 02 Apr 2021 18:20:13 GMT  
		Size: 300.4 KB (300408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ded8b3705333f72888d4cf854eb5f4940ce814721660bbd55d109a8826a03`  
		Last Modified: Fri, 02 Apr 2021 18:20:14 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afb4b7cde85cac613122e5ebf2d7f97cdc4457913475e0af127a9ad83467baf`  
		Last Modified: Fri, 02 Apr 2021 18:20:15 GMT  
		Size: 11.4 MB (11407320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44ff6c0ff0fd070875236cb70163a5b5d10a6c91a029e468a1b507939aca9a`  
		Last Modified: Fri, 02 Apr 2021 18:20:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:aa5fedf546f66c9c7479220756a01f8ca9c421a5e78117db86fc54c14bb340cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13740480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be8c4334d684912f0cae439c7fb5d51334993ca3b5c417380b4b35e63b29f1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Fri, 02 Apr 2021 18:49:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:49:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:49:55 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:50:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:50:12 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:50:14 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:50:16 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:50:18 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:50:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:50:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:50:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:50:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:50:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:50:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:50:48 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:50:53 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:50:55 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:50:58 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:51:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1e1bc72d95e03e28e991fa53bb7f7238ffd16a125465b7a73ef9f68a4484bd`  
		Last Modified: Fri, 02 Apr 2021 18:52:14 GMT  
		Size: 300.5 KB (300514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99f0b778282aad6bc6b2e941fec2708198912824fd2ca2a0ae63ff9920bd387`  
		Last Modified: Fri, 02 Apr 2021 18:52:14 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1263c98147d8e73b762bb9ae4979f3c6eaecb780937aa25344f7a8f26734b09`  
		Last Modified: Fri, 02 Apr 2021 18:52:18 GMT  
		Size: 10.8 MB (10811865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379c3d17de6d89ea87e3f4b22fee1451995467ceafe97afb45ff52d6c391ada1`  
		Last Modified: Fri, 02 Apr 2021 18:52:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8977e27736ba1604ad1d09d8ad8c19324842597ddfd01ef8a91f754a308be597
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13522013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b879077000bbeb58c1b52b2fc34fd349f34a2376856dbaa2f9fc886ff4a9c4ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:12:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:59:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:59:41 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:59:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 19:00:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 19:00:16 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 19:00:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 19:00:22 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 19:00:30 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 19:00:36 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 19:00:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 19:00:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 19:00:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 19:00:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 19:00:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 19:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 19:01:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 19:01:23 GMT
EXPOSE 80
# Fri, 02 Apr 2021 19:01:30 GMT
EXPOSE 443
# Fri, 02 Apr 2021 19:01:42 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 19:02:07 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 19:02:10 GMT
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
	-	`sha256:447e6bb723906fc976d81f3c33ba05a5541e43675b2ef9c40091303bb8bddb04`  
		Last Modified: Fri, 02 Apr 2021 19:05:04 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017a0481e097bef99cf346fa602697e6ec6e92dd192bfc8154f4a48f26ab7422`  
		Last Modified: Fri, 02 Apr 2021 19:05:09 GMT  
		Size: 10.8 MB (10792254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5166e8b56ad50e701cf797364485ea83aee29b1f3adceb2ba10c24fc86bdb011`  
		Last Modified: Fri, 02 Apr 2021 19:05:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6d943c417dacd177b0c1ba339a4699945e2a2d1e5de410460c1545e456d7ffb5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13377671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8713774d73974c29e36ee5bb9196c9bdc2f54b27b748621ed957dbcbb53350`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:42:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:44:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:44:47 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:44:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:45:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:45:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:45:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:45:19 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:45:29 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:45:34 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:45:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:45:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:45:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:45:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:46:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:46:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:46:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:46:39 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:46:45 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:46:53 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:47:23 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:47:37 GMT
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
	-	`sha256:ac03593c77aa97dc2b49138e6c2d64e0d2b549487cbfa8be194df575919d86d4`  
		Last Modified: Fri, 02 Apr 2021 18:49:29 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8282ed2393080ee9fbccf1fb5ecdb56aa5178da9dfe1479cfcfa4b49f07dfd`  
		Last Modified: Fri, 02 Apr 2021 18:49:32 GMT  
		Size: 10.4 MB (10359151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b147e37453b43e707911e9e1182ab653ef4e42411bf2dbf030f61f7b5543f1`  
		Last Modified: Fri, 02 Apr 2021 18:49:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2` - linux; ppc64le

```console
$ docker pull caddy@sha256:69bf6d485cca04a1d5b497061ff8a3465aab5a0f56aa14e09c9840d73deeb557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13079861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b36fb90d1135bfbf325f21736498234b14ee036830d05b110230f91a7b2c873`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:23:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:19:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:20:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:21:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:21:30 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:21:54 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:22:17 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:22:36 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:22:43 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:22:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:23:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:23:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:23:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:23:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:23:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:23:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:23:48 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:23:56 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:24:05 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:24:15 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:24:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd67c6c19ed1d5aad6173157b10ed430dc4b79f7aefd9b15968e3d6f2515ef8`  
		Last Modified: Thu, 01 Apr 2021 20:28:17 GMT  
		Size: 302.5 KB (302540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446396dbb30a2925d80e617fbeabd659f039220522d910dd811c13927bf36c2a`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977297ea362b91438c0d23b7a5e054d023732d70ff45dbf0e856b88504a5a0d5`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 10.0 MB (9958115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ddb1940c4a291b09e86d1f35f1591e61597f37f91859016cf0e28f91f46c2`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2` - linux; s390x

```console
$ docker pull caddy@sha256:c093c6df07e976c6544777eef3dbec8efb22231132046ef67a400bad8b75083f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13897301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b2cdf76b47d28ab04dfb908fcd67535e75e5c3ccf8867fc11e928f3e97c1b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Fri, 02 Apr 2021 18:41:35 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:41:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:41:37 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:41:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:41:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:41:40 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:41:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:41:40 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:41:41 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:41:41 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:41:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:41:43 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:41:43 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:41:43 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:41:43 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:41:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bdee00e0d42aa0eac225d6882199a22161798072f0c25e30b7b4b8896545cc`  
		Last Modified: Fri, 02 Apr 2021 18:42:14 GMT  
		Size: 300.8 KB (300829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070fe2ada5f147f27af3e4a6091cc3f466f9af385177076a766396c3e2634c02`  
		Last Modified: Fri, 02 Apr 2021 18:42:15 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8391d5bf2258305005739ed98cbb49ec466fc95757fa0cb14f40a89262ffe13e`  
		Last Modified: Fri, 02 Apr 2021 18:42:16 GMT  
		Size: 11.0 MB (10987897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6dd4c5ad3aa33d5340696408e521f09c1cfc35c26779f22707d51ccc50809c`  
		Last Modified: Fri, 02 Apr 2021 18:42:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:6f39355785ee4e6f020cd3755adb37e0f09f396afd9fcaa7330e15d424e225b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487602702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11dbe1305e7cbce4d507512474f6d9c114c88ecf4c1e6ac3802065b47d6c175c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:16:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 02 Apr 2021 18:16:24 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:16:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9f41c88fc8c2c28230c5eb67fb7d9ef23477a351fb716a44486b3d1a37569fb141112cd3582adcd44424b2819c22723fb49023a6d371e1bf8d92eefe4e7e9ed4')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 02 Apr 2021 18:16:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 02 Apr 2021 18:16:56 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 02 Apr 2021 18:16:58 GMT
VOLUME [c:/config]
# Fri, 02 Apr 2021 18:16:59 GMT
VOLUME [c:/data]
# Fri, 02 Apr 2021 18:17:00 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:17:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:17:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:17:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:17:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:17:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:17:09 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:17:10 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:17:11 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:17:29 GMT
RUN caddy version
# Fri, 02 Apr 2021 18:17:30 GMT
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
	-	`sha256:95e2248c328b7b25c2cbbab7676a8e86d131ea6ad52f5f7bd35647a14893a0a2`  
		Last Modified: Fri, 02 Apr 2021 18:25:36 GMT  
		Size: 9.5 MB (9465706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94271d4a9ce601138f36c7f2d749d748b9ced3d0f52764ca356d32860edb5c5`  
		Last Modified: Fri, 02 Apr 2021 18:25:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ca5665516d898633290e493cef794521852475d69230732409986f3ad81705`  
		Last Modified: Fri, 02 Apr 2021 18:25:38 GMT  
		Size: 16.3 MB (16274695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de70870a5fa3de27854447c44c6ba786981cc938c0f362048da4170553463a`  
		Last Modified: Fri, 02 Apr 2021 18:25:32 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3568445127d07f06bf99e10ae664cca603cc31e68c728060dcac8f7e608881`  
		Last Modified: Fri, 02 Apr 2021 18:25:32 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da65ebebad5059d100ae2af112ca25285129bee6131023aa4c8ce7f0f830793a`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48067c5e57f31ce03ffc3422870602c673527153e446f55fe44dc813bebf9b4`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f2e781673fc6a350cf8b08667e71ffdf90d42f5b0a6a1d9da8e29771f1ffc6`  
		Last Modified: Fri, 02 Apr 2021 18:25:29 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8493be2eceb4e6ea31b450a179859bfd185e92ffd3bbf301fcbd9cb409bcb911`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7a94659f6ba05b7478802b8b57b48e51bbc397ddd845b315891c3e32c1be32`  
		Last Modified: Fri, 02 Apr 2021 18:25:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0db2eb1ebe3b7e3abc59d777a66b0b0b8f51cb3378cc265655f1bfcd7e79312`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6c27364edfca6e69e47b72493bac0aa0242ed5630222b468f2511911e9db14`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ed9f38d63bbcecb70291bbc12286363d05cd6e3fb4be3863ea7332dfd32df8`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b92c3fb781472d906952c139a15a924de551954360d972757c2b7fa70127fc7`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc395ee40c1f92ebe4a8630100e8e3a0323cd404b6e2b4a13b8cd01e17514c1`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daab2d67688cedff5bdcbd07535b3be37f2493b23cd92a902e0f241d46be09f`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc8f200f7b9a010feb0546619b1dee830f1b1ec0dc747ad7158ecb0088482c`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd8989a8ea6c4f623b19785b82af238aee316ee6b72e732262a87011c74d62`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d6b1aa36e5bfef2dfa42970c937fc34573ad9f72508693cda371163b8da379`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 302.3 KB (302255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ec29f6e55d821e399842d426dab17fde9d0ddebeb312cbb9e2a7c07cbdf0b3`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:484c688cb48fa269829e7f6b85bc623bc1b5061043c0e673cc323ccb7c465abc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829094060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86b0dff6059a7f821d34de02f7303fd43d1f41212c68037dd2876ebd5663e534`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:19:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 02 Apr 2021 18:19:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9f41c88fc8c2c28230c5eb67fb7d9ef23477a351fb716a44486b3d1a37569fb141112cd3582adcd44424b2819c22723fb49023a6d371e1bf8d92eefe4e7e9ed4')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 02 Apr 2021 18:20:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 02 Apr 2021 18:20:47 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 02 Apr 2021 18:20:48 GMT
VOLUME [c:/config]
# Fri, 02 Apr 2021 18:20:49 GMT
VOLUME [c:/data]
# Fri, 02 Apr 2021 18:20:50 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:20:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:20:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:20:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:20:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:20:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:21:00 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:21:01 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:21:02 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:21:57 GMT
RUN caddy version
# Fri, 02 Apr 2021 18:21:58 GMT
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
	-	`sha256:3839f3b2a37673d4006f18951ce8d65dac9f9e7a60c481cf4fa86898372bcc72`  
		Last Modified: Fri, 02 Apr 2021 18:25:59 GMT  
		Size: 10.2 MB (10196223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35d02bac712107cd6e45e8ecf4c379e9fe8ba144b8b1af73c9fbaeeb9b5ea21`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f861c5228e163fdd027d65ffdb9bf65e90a1940df415ad2c0ce25ab35cd093`  
		Last Modified: Fri, 02 Apr 2021 18:26:01 GMT  
		Size: 21.7 MB (21693316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f4820276b1680a1ec83d16ac48637c3bb3a276c31baaaf17dd757edd9f4188`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d3d58a6632e499c498ca0addf11c2b22067f5427a93e69885d6b38e1b10596`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28b4d2afe9acc4864ab15a603e8672fb2482c1dd648c57e32456bf7765c3c63`  
		Last Modified: Fri, 02 Apr 2021 18:25:53 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6489ff70b21ce91518922c0d1bfd94e89f92403b67f5a24a1825fd37f28f5aaf`  
		Last Modified: Fri, 02 Apr 2021 18:25:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c0ad8640bb2534d11d722e0777eca31ac10db266abae4cbeefcdfc9f1936a8`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7885acef6da7eb82e08e66cab23b2890f3f3dafef9ec189e81f8045c1954afc`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1f28035d278c150033dbc5d05f6fa9dd3ece81bba6b2a85b3453414398f8aa`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19f2df18981d5ee49e3c45183b1d251f5c4ab848c5f6dc0c0816224f900d287`  
		Last Modified: Fri, 02 Apr 2021 18:25:50 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786ed8d22ae84118b965493f2dc3e79c27bb76f8e34470a569d40d5b9197d008`  
		Last Modified: Fri, 02 Apr 2021 18:25:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b1cde58cdb206802bae3748fc1791648ec167a9addfc05d71af8ef80a7263`  
		Last Modified: Fri, 02 Apr 2021 18:25:49 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a08c62e43e038c439e7b271c524bc1b032913ef0a7838c7a28574564267f4d`  
		Last Modified: Fri, 02 Apr 2021 18:25:48 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629328a7926be76a0105b548d269200ac4213b329ac924c6dc34399747a0a6e4`  
		Last Modified: Fri, 02 Apr 2021 18:25:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b6aec700c2791f546afb2dc6d5045b6ea036c6117b574d5ed06454a2eb5e42`  
		Last Modified: Fri, 02 Apr 2021 18:25:47 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ded6ed75772c3a5c3485bda081d2914ed7b8b0850d62e3d9b9dcfcb86b97961`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55d3e22aa51f274d765555ceb7acfe4c95dfdf06ed747cb78ff3955ec37b43a`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1282f41e60a0e981888559572f13a307d872bb4fb6d636ea2af4a71aa953d4`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 268.3 KB (268326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a7b2d83b6c9a47753c8f82981aefe854fefc34fa7f1ee836fd656fc47f38d`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-alpine`

```console
$ docker pull caddy@sha256:4ad8e0a84f1ca92a6d8bb3e956dd6443ecc44ef717c104c8ef089da88860f769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.0-beta.2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:fa50efe45a26d4e0d4ee53589eefc94adc848e23599088e3a23fa8a46e37b0ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14525653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c90ba77981732d04067f9d48287ef8cabe5c59a33c4561d4668fbe43695bc0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Fri, 02 Apr 2021 18:19:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:19:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:19:34 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:19:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:19:38 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:19:38 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:19:38 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:19:38 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:19:38 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:19:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:19:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:19:40 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:19:40 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:19:40 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:19:41 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:19:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212f6a1c9e4977bde3df77a8a6c46bf7757d599f51a15eb01c63bd2be543cb40`  
		Last Modified: Fri, 02 Apr 2021 18:20:13 GMT  
		Size: 300.4 KB (300408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5ded8b3705333f72888d4cf854eb5f4940ce814721660bbd55d109a8826a03`  
		Last Modified: Fri, 02 Apr 2021 18:20:14 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afb4b7cde85cac613122e5ebf2d7f97cdc4457913475e0af127a9ad83467baf`  
		Last Modified: Fri, 02 Apr 2021 18:20:15 GMT  
		Size: 11.4 MB (11407320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44ff6c0ff0fd070875236cb70163a5b5d10a6c91a029e468a1b507939aca9a`  
		Last Modified: Fri, 02 Apr 2021 18:20:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:aa5fedf546f66c9c7479220756a01f8ca9c421a5e78117db86fc54c14bb340cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13740480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be8c4334d684912f0cae439c7fb5d51334993ca3b5c417380b4b35e63b29f1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Fri, 02 Apr 2021 18:49:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:49:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:49:55 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:50:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:50:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:50:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:50:12 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:50:14 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:50:16 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:50:18 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:50:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:50:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:50:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:50:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:50:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:50:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:50:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:50:48 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:50:53 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:50:55 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:50:58 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:51:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1e1bc72d95e03e28e991fa53bb7f7238ffd16a125465b7a73ef9f68a4484bd`  
		Last Modified: Fri, 02 Apr 2021 18:52:14 GMT  
		Size: 300.5 KB (300514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99f0b778282aad6bc6b2e941fec2708198912824fd2ca2a0ae63ff9920bd387`  
		Last Modified: Fri, 02 Apr 2021 18:52:14 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1263c98147d8e73b762bb9ae4979f3c6eaecb780937aa25344f7a8f26734b09`  
		Last Modified: Fri, 02 Apr 2021 18:52:18 GMT  
		Size: 10.8 MB (10811865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379c3d17de6d89ea87e3f4b22fee1451995467ceafe97afb45ff52d6c391ada1`  
		Last Modified: Fri, 02 Apr 2021 18:52:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8977e27736ba1604ad1d09d8ad8c19324842597ddfd01ef8a91f754a308be597
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13522013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b879077000bbeb58c1b52b2fc34fd349f34a2376856dbaa2f9fc886ff4a9c4ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 08:12:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:59:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:59:41 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:59:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 19:00:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 19:00:16 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 19:00:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 19:00:22 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 19:00:30 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 19:00:36 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 19:00:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 19:00:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 19:00:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 19:00:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 19:00:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 19:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 19:01:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 19:01:23 GMT
EXPOSE 80
# Fri, 02 Apr 2021 19:01:30 GMT
EXPOSE 443
# Fri, 02 Apr 2021 19:01:42 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 19:02:07 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 19:02:10 GMT
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
	-	`sha256:447e6bb723906fc976d81f3c33ba05a5541e43675b2ef9c40091303bb8bddb04`  
		Last Modified: Fri, 02 Apr 2021 19:05:04 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017a0481e097bef99cf346fa602697e6ec6e92dd192bfc8154f4a48f26ab7422`  
		Last Modified: Fri, 02 Apr 2021 19:05:09 GMT  
		Size: 10.8 MB (10792254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5166e8b56ad50e701cf797364485ea83aee29b1f3adceb2ba10c24fc86bdb011`  
		Last Modified: Fri, 02 Apr 2021 19:05:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6d943c417dacd177b0c1ba339a4699945e2a2d1e5de410460c1545e456d7ffb5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13377671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8713774d73974c29e36ee5bb9196c9bdc2f54b27b748621ed957dbcbb53350`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 12:42:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:44:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:44:47 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:44:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:45:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:45:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:45:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:45:19 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:45:29 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:45:34 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:45:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:45:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:45:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:45:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:46:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:46:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:46:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:46:39 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:46:45 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:46:53 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:47:23 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:47:37 GMT
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
	-	`sha256:ac03593c77aa97dc2b49138e6c2d64e0d2b549487cbfa8be194df575919d86d4`  
		Last Modified: Fri, 02 Apr 2021 18:49:29 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8282ed2393080ee9fbccf1fb5ecdb56aa5178da9dfe1479cfcfa4b49f07dfd`  
		Last Modified: Fri, 02 Apr 2021 18:49:32 GMT  
		Size: 10.4 MB (10359151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b147e37453b43e707911e9e1182ab653ef4e42411bf2dbf030f61f7b5543f1`  
		Last Modified: Fri, 02 Apr 2021 18:49:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:69bf6d485cca04a1d5b497061ff8a3465aab5a0f56aa14e09c9840d73deeb557
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13079861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b36fb90d1135bfbf325f21736498234b14ee036830d05b110230f91a7b2c873`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:23:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:19:53 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:20:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:21:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:21:30 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:21:54 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:22:17 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:22:36 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:22:43 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:22:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:23:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:23:11 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:23:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:23:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:23:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:23:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:23:48 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:23:56 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:24:05 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:24:15 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:24:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd67c6c19ed1d5aad6173157b10ed430dc4b79f7aefd9b15968e3d6f2515ef8`  
		Last Modified: Thu, 01 Apr 2021 20:28:17 GMT  
		Size: 302.5 KB (302540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446396dbb30a2925d80e617fbeabd659f039220522d910dd811c13927bf36c2a`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977297ea362b91438c0d23b7a5e054d023732d70ff45dbf0e856b88504a5a0d5`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 10.0 MB (9958115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304ddb1940c4a291b09e86d1f35f1591e61597f37f91859016cf0e28f91f46c2`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c093c6df07e976c6544777eef3dbec8efb22231132046ef67a400bad8b75083f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13897301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b2cdf76b47d28ab04dfb908fcd67535e75e5c3ccf8867fc11e928f3e97c1b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Fri, 02 Apr 2021 18:41:35 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 02 Apr 2021 18:41:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"
# Fri, 02 Apr 2021 18:41:37 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:41:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41daeac683d503264496689c6271645293c95518c5b97870c3f3a17127ae35b820622720315901c0c5856b42e0201b7eaad153dfa4a1045502a99f41d0b9785d' ;; 		armhf)   binArch='armv6'; checksum='51e4d7220064e1948232c8c54996b012d01fe0e2caa71200e34f0da59bd6267cdc318124e1a7a44e83ce54b7276f6d0fb32381d3080e05902d3c3528ff423dd7' ;; 		armv7)   binArch='armv7'; checksum='9c3b4eea4840a1fe633d45d436789edf6839e96527783d2eac309d24e5085c0cdee8beffd7e5ad2f1d7d31e16004e916aa29456d8ac52007e9d904e644d6db40' ;; 		aarch64) binArch='arm64'; checksum='86cf83d11aee266d32c262982df3e286aa0a4b391fc4fbded0e299ace043c753e9a1f53bef1f95a292a71107e1f9578a8615b038871eedb171437eebe7db47d2' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='81b050dae2892feb517db6c782acc506dfe21399b0a79073e5191656f57c6d0a5a511caf1086ffc671712ab198715cca6a2a120812a4df8d774ba17d6242aa39' ;; 		s390x)   binArch='s390x'; checksum='763256d267ad8832c37fa1a902fc06dfb6b9871b75e38545cbc199b50251f78b0cc2400104d31fc18d2c98408f02a74e581a7f7746974837dcdef51a4a259bf2' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 02 Apr 2021 18:41:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 02 Apr 2021 18:41:40 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 02 Apr 2021 18:41:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 02 Apr 2021 18:41:40 GMT
VOLUME [/config]
# Fri, 02 Apr 2021 18:41:41 GMT
VOLUME [/data]
# Fri, 02 Apr 2021 18:41:41 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:41:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:41:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:41:43 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:41:43 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:41:43 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:41:43 GMT
WORKDIR /srv
# Fri, 02 Apr 2021 18:41:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bdee00e0d42aa0eac225d6882199a22161798072f0c25e30b7b4b8896545cc`  
		Last Modified: Fri, 02 Apr 2021 18:42:14 GMT  
		Size: 300.8 KB (300829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070fe2ada5f147f27af3e4a6091cc3f466f9af385177076a766396c3e2634c02`  
		Last Modified: Fri, 02 Apr 2021 18:42:15 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8391d5bf2258305005739ed98cbb49ec466fc95757fa0cb14f40a89262ffe13e`  
		Last Modified: Fri, 02 Apr 2021 18:42:16 GMT  
		Size: 11.0 MB (10987897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6dd4c5ad3aa33d5340696408e521f09c1cfc35c26779f22707d51ccc50809c`  
		Last Modified: Fri, 02 Apr 2021 18:42:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-builder`

```console
$ docker pull caddy@sha256:e2a29e282dc9bf0a2441c771d577b438c1e6671b45b6bed959bac282a4a0a131
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

### `caddy:2.4.0-beta.2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:c1498c04ecceb6146f0ca7b3261a6adc6d688baf36d1f09d18f7d80581b11b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116492995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75a312935a69cd4fa902f97b4505ecfb64268fc78410c17e925fef00670ac9a`
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
# Fri, 02 Apr 2021 00:20:32 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:22:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:22:14 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:22:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:22:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:22:15 GMT
WORKDIR /go
# Fri, 02 Apr 2021 18:19:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 18:19:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:19:46 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:19:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:19:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:19:48 GMT
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
	-	`sha256:3e4189aff30b2bf70434e47d0fccc5279d2f419c2068c8a6bb5b4335f14fcc79`  
		Last Modified: Fri, 02 Apr 2021 00:30:58 GMT  
		Size: 105.7 MB (105700168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24a58abccf63630e7b73e77f5de1baa44a61254aee1aef202fea1e6217f2adb`  
		Last Modified: Fri, 02 Apr 2021 00:30:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd14866198080cff5f46908b8431bb3ea882aa069e4ad36faaaad855f2394cb9`  
		Last Modified: Fri, 02 Apr 2021 18:20:24 GMT  
		Size: 6.4 MB (6387824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4944b6dcebcd2e315c2adca56e09b2dcb43ca77be4d8f31d2f9913e15edc4d87`  
		Last Modified: Fri, 02 Apr 2021 18:20:24 GMT  
		Size: 1.3 MB (1311067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2139e18074e3608d84872445ae127d38efc607b1512beec51afc70a718a09dfc`  
		Last Modified: Fri, 02 Apr 2021 18:20:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:64011587ef8b76a2996a366297c2765fa6d210b957bb6e33bcd04d0e7d14ca44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112258744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dc62dbacffb03fcd969ab44f14115ecd014d590050ebdc3906629840f3c25c7`
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
# Thu, 01 Apr 2021 23:52:23 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:36:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:36:27 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:36:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:36:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:37:09 GMT
WORKDIR /go
# Fri, 02 Apr 2021 18:51:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 18:51:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:51:29 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:51:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:51:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:51:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:51:44 GMT
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
	-	`sha256:e606a127afa4cc828abd4312986157fcf53462f7fe42cda550887c0b5baea0d0`  
		Last Modified: Fri, 02 Apr 2021 01:35:00 GMT  
		Size: 101.9 MB (101907855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f706960818fa687848bd9ba6d330cf40b5825a42207c41289d143dd8c59819a0`  
		Last Modified: Fri, 02 Apr 2021 01:34:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6204569d16950272d1853adbcfb2af8cc17033fed68529720ed9f041e7beb77`  
		Last Modified: Fri, 02 Apr 2021 18:52:25 GMT  
		Size: 6.2 MB (6225098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f209cd8964e286ecac9428fb49ed823e896ea8028be622275772aa01bc97864`  
		Last Modified: Fri, 02 Apr 2021 18:52:23 GMT  
		Size: 1.2 MB (1221589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee602665c1713065c6eead979fd462f942b7d7189161df8168b23a4ab5c5c1b0`  
		Last Modified: Fri, 02 Apr 2021 18:52:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:73bbbb1238c100177fb2bc24bcac1b599c45de279d9b0c5c8b73869b1b36db0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111181631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98212955f480b1c834167f05d6221b7340f518364424ce63e375263e343b4613`
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
# Fri, 02 Apr 2021 00:09:57 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:52:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:52:49 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:53:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:53:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:54:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:40:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:40:08 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 19:02:27 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 19:02:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 19:02:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 19:03:19 GMT
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
	-	`sha256:de79052905e4120d804a4aac99d4f39ba3e122ac3c75efe8363ad5adf256f927`  
		Last Modified: Fri, 02 Apr 2021 01:43:50 GMT  
		Size: 101.7 MB (101698695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c365eb52b58a9023f2a7c4766d48472e0a447c37c43cb6ad323f2cc8d6c1c`  
		Last Modified: Fri, 02 Apr 2021 01:42:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6214666ea97e54cb4b48c6e316c3542dd3cdee7f0473e72572c8bc3eacea93`  
		Last Modified: Fri, 02 Apr 2021 03:40:56 GMT  
		Size: 5.6 MB (5558125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9e094ef99cac0175242d7df4a1381918a7c602cc591dbf623d401e1fb1a711`  
		Last Modified: Fri, 02 Apr 2021 19:05:30 GMT  
		Size: 1.2 MB (1219458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40c204ad1fccd1c6eb4773005a7f7219ec24d3926ffef501f6adcceeefbc61b`  
		Last Modified: Fri, 02 Apr 2021 19:05:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:08eaf7a5776da557c1db6c274e87475695fa4698d7b43c7940b8bbecf247915a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111710773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a97900c49d5b44c8c352da00af28fec5f19dcd3788e7612931c0c0a2f57bc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:36:18 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:36:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:36:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:44:23 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:48:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:49:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:37 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:39:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:39:18 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:48:03 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:48:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:48:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:48:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:48:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d3c479d6df2bd83adc83bbac78968bfb4e1abcf6fe557f118b9209078d2ad7`  
		Last Modified: Thu, 01 Apr 2021 16:47:42 GMT  
		Size: 281.5 KB (281483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ae0fd282dc382614f6f786d6a0fc72ed7f4b2054371020563e3e69df43b012`  
		Last Modified: Thu, 01 Apr 2021 16:47:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b472b1c93ad35dfad1b4e65e64156f0f44aa1fe7f105a2d55047d5238852`  
		Last Modified: Fri, 02 Apr 2021 01:13:47 GMT  
		Size: 101.0 MB (101041047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8038507963aca0d9a0c18e8e1870c46927fa6301b0b78be430c58c5e396bee2`  
		Last Modified: Fri, 02 Apr 2021 01:13:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17c1acee68686ada56220f5be4f872287caabbc3f1bc839e349bd00fccad975`  
		Last Modified: Fri, 02 Apr 2021 02:40:36 GMT  
		Size: 6.5 MB (6474039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7484fe4a43db2e2499090ce4f4c7c3af60193ba8366a7e562acba334b1fc0322`  
		Last Modified: Fri, 02 Apr 2021 18:49:42 GMT  
		Size: 1.2 MB (1201567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df5e6b067c7995a06f0f74ef2fc94adb9f26adf36db39dfd86f259db453eae`  
		Last Modified: Fri, 02 Apr 2021 18:49:42 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:beafcff354118be6cd1946efd9ca2028d36de418a510abc6c65321c08f116a63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110604319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40416b4b95b5338e9d6917f544078a6208c1f7fb7e2620b32fb40c053a634b1e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:30:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:30:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:09:14 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 03:11:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:11:20 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:11:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:11:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:11:51 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:24:35 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:24:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:24:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:24:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:24:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc638e60e2f17921f3b4535edbf7095cc97278ba8d1410fd7e018101a1242be3`  
		Last Modified: Thu, 01 Apr 2021 04:44:03 GMT  
		Size: 283.4 KB (283416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b706ed0ac7a9324a306982c3913517f4f044be650413df529bf27a05c288d1b9`  
		Last Modified: Thu, 01 Apr 2021 04:44:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b169d190e0156b6deab2ff0e58a47150fc50f2868a89d84eb61c9570305e930`  
		Last Modified: Fri, 02 Apr 2021 03:23:03 GMT  
		Size: 99.5 MB (99513251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83adeb4b646f1b8b0b72cac1632f1bddf6a8b5499291eb0fec11957739b98ec1`  
		Last Modified: Fri, 02 Apr 2021 03:22:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604836dc523b402ec6de96489b450d95b267f41ae391d700d4d21b759ffde953`  
		Last Modified: Fri, 02 Apr 2021 05:04:42 GMT  
		Size: 6.8 MB (6823220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4317a229e7753654e9d8b6b11dae3b5cb7be5941f353851b897405e9846c4d56`  
		Last Modified: Fri, 02 Apr 2021 18:25:36 GMT  
		Size: 1.2 MB (1170495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44a0398c5bef844d519cc025aa24a3ebf5343578a6bb8b3632cad3f0842284e`  
		Last Modified: Fri, 02 Apr 2021 18:25:36 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:d363d8e70a8277c2cd56a4cdf4c9527b06097d4f7289a9386ce4c8930246bb01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115430971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf585bf0a2c7796ab5124b11aee2e6b61436fb1e98d0061ffc1414e4b77f54d`
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
# Fri, 02 Apr 2021 00:42:03 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:43:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:43:36 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:43:37 GMT
WORKDIR /go
# Fri, 02 Apr 2021 18:41:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 18:41:50 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:41:50 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:41:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:41:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:41:52 GMT
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
	-	`sha256:d84d135a3d538231dcbc75989d5cb96ac1fd2d8aafd066e7d696d295d4252940`  
		Last Modified: Fri, 02 Apr 2021 00:50:10 GMT  
		Size: 104.8 MB (104809692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de86cbaefc9f6a24519f984378bc3ea0033c6767c5cfa28afeb50edc9a86c5f`  
		Last Modified: Fri, 02 Apr 2021 00:49:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65369d0863ca497de787c86268a4c35482ace4570eabbba157106b2895427ed7`  
		Last Modified: Fri, 02 Apr 2021 18:42:22 GMT  
		Size: 6.5 MB (6471846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9682c6a1905e52c629b4a35d0b39e7c2ff1467d4366a479416007c844fdb4fc6`  
		Last Modified: Fri, 02 Apr 2021 18:42:22 GMT  
		Size: 1.3 MB (1264432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f7f3cd797d6b812a051ae4023b788dc562657b43de6f56c3bffc732a702f40`  
		Last Modified: Fri, 02 Apr 2021 18:42:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:9d285ead4bdf8f99fedfbe03501c691819e48f831e0b0084580a59cb8bf0bad4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2641868622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c93dc0b0fa48b343cd322c901f869fc6a46e264b6256d2fec7f4be8f2b219e04`
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
# Fri, 02 Apr 2021 00:15:25 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:18:07 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'a4400345135b36cb7942e52bbaf978b66814738b855eeff8de879a09fd99de7f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:18:09 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 18:22:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:22:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:22:09 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:22:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:22:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 18:22:38 GMT
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
	-	`sha256:9a7e34d0221e19de26b1af5fb6e32ddd3d7af02c7da8f8797c0b1d88608c507e`  
		Last Modified: Fri, 02 Apr 2021 00:36:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7c9e37d4f37ac6c3bbb4a4ea26623159bd41ab01eeb97ba5f3558f6f0b2e6c`  
		Last Modified: Fri, 02 Apr 2021 00:36:59 GMT  
		Size: 143.7 MB (143721828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14239a8d1f9055a3b8d9d966990a90be84c447b26212c8c31746315beb5af592`  
		Last Modified: Fri, 02 Apr 2021 00:36:22 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cf60572a4ce4c53cd6b737d1d0052857aefd64967385c2dfb51ca7ab737d87`  
		Last Modified: Fri, 02 Apr 2021 18:26:11 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb15e0f080d4ffebac67b5651ae2308c376db5d2c6d35645ce7a3df70088d1a`  
		Last Modified: Fri, 02 Apr 2021 18:26:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933d5696db6c53091e2d4ec83ddc685bd4ac95836dc1adc50e05ed712658a869`  
		Last Modified: Fri, 02 Apr 2021 18:26:08 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa8b4229fc77631db90295128b3ee38f226ce9855444819dde0ec638023b873`  
		Last Modified: Fri, 02 Apr 2021 18:26:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42288aa25a7176680ab6a682e44da10f14581942c25ed0cddc0827b54cae0bad`  
		Last Modified: Fri, 02 Apr 2021 18:26:09 GMT  
		Size: 1.7 MB (1714787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284cd2af3a6274b07a526bf01c7021477428137fd0f4938856f2a10d5dc78d0e`  
		Last Modified: Fri, 02 Apr 2021 18:26:12 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:c1cfba3a3aa32a96fa4d6b325e56473c26a28d6f3db68ba2d8704a3fc1be6c49
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6003045589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79ee0f3301ee81e21e378ce3f53b7305e6e3db4119c6f6bc1e8ab85411402213`
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
# Fri, 02 Apr 2021 00:18:24 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:22:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'a4400345135b36cb7942e52bbaf978b66814738b855eeff8de879a09fd99de7f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:22:43 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 18:22:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:22:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:22:47 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:22:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:24:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 18:24:20 GMT
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
	-	`sha256:5e7c38f99787bf274ac0a56d06ab8d5ada8675bdbc1b8a41ac4e8e005be67cf3`  
		Last Modified: Fri, 02 Apr 2021 00:37:20 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858a80496ac8841bb47d698f77d63b80c5bfb5c71f3e836cd63729731eb2d0c3`  
		Last Modified: Fri, 02 Apr 2021 00:40:16 GMT  
		Size: 149.2 MB (149164836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f6bce455ff0310e2c186805aff8794f0ae69ed9bac6df06f7f6240d1ba4212`  
		Last Modified: Fri, 02 Apr 2021 00:37:20 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6470d57243826b35d3959d11a867738f749a6118e42d9881bae1d6d022b5cd`  
		Last Modified: Fri, 02 Apr 2021 18:26:22 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2dc30f3688f8d90d917c010cffed48167b0a15f018655d85d79ffc5b7522885`  
		Last Modified: Fri, 02 Apr 2021 18:26:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d18daa399267ca08468b3402c46122b9aa3e5e80c7fb1860558585100eca16c`  
		Last Modified: Fri, 02 Apr 2021 18:26:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcedff24a492766afee3560aca62ebae75ec3a54f253d95c44247b79d24b27a`  
		Last Modified: Fri, 02 Apr 2021 18:26:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d328d81e64b61062f2891b3c48b51ccb4badcbe1efc420c2acbfc43938f5d5ef`  
		Last Modified: Fri, 02 Apr 2021 18:26:25 GMT  
		Size: 11.5 MB (11539007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228dc315d7ba3fe405accce7eafdd95cd5861cda759a223fae2852cceaa01213`  
		Last Modified: Fri, 02 Apr 2021 18:26:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-builder-alpine`

```console
$ docker pull caddy@sha256:f35b9113aef39447cad062b84ee855f3f781e45e27ed27169d98b5c7f8d0f0e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.0-beta.2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:c1498c04ecceb6146f0ca7b3261a6adc6d688baf36d1f09d18f7d80581b11b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116492995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75a312935a69cd4fa902f97b4505ecfb64268fc78410c17e925fef00670ac9a`
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
# Fri, 02 Apr 2021 00:20:32 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:22:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:22:14 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:22:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:22:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:22:15 GMT
WORKDIR /go
# Fri, 02 Apr 2021 18:19:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 18:19:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:19:46 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:19:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:19:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:19:48 GMT
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
	-	`sha256:3e4189aff30b2bf70434e47d0fccc5279d2f419c2068c8a6bb5b4335f14fcc79`  
		Last Modified: Fri, 02 Apr 2021 00:30:58 GMT  
		Size: 105.7 MB (105700168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24a58abccf63630e7b73e77f5de1baa44a61254aee1aef202fea1e6217f2adb`  
		Last Modified: Fri, 02 Apr 2021 00:30:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd14866198080cff5f46908b8431bb3ea882aa069e4ad36faaaad855f2394cb9`  
		Last Modified: Fri, 02 Apr 2021 18:20:24 GMT  
		Size: 6.4 MB (6387824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4944b6dcebcd2e315c2adca56e09b2dcb43ca77be4d8f31d2f9913e15edc4d87`  
		Last Modified: Fri, 02 Apr 2021 18:20:24 GMT  
		Size: 1.3 MB (1311067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2139e18074e3608d84872445ae127d38efc607b1512beec51afc70a718a09dfc`  
		Last Modified: Fri, 02 Apr 2021 18:20:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:64011587ef8b76a2996a366297c2765fa6d210b957bb6e33bcd04d0e7d14ca44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112258744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dc62dbacffb03fcd969ab44f14115ecd014d590050ebdc3906629840f3c25c7`
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
# Thu, 01 Apr 2021 23:52:23 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:36:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:36:27 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:36:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:36:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:37:09 GMT
WORKDIR /go
# Fri, 02 Apr 2021 18:51:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 18:51:26 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:51:29 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:51:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:51:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:51:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:51:44 GMT
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
	-	`sha256:e606a127afa4cc828abd4312986157fcf53462f7fe42cda550887c0b5baea0d0`  
		Last Modified: Fri, 02 Apr 2021 01:35:00 GMT  
		Size: 101.9 MB (101907855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f706960818fa687848bd9ba6d330cf40b5825a42207c41289d143dd8c59819a0`  
		Last Modified: Fri, 02 Apr 2021 01:34:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6204569d16950272d1853adbcfb2af8cc17033fed68529720ed9f041e7beb77`  
		Last Modified: Fri, 02 Apr 2021 18:52:25 GMT  
		Size: 6.2 MB (6225098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f209cd8964e286ecac9428fb49ed823e896ea8028be622275772aa01bc97864`  
		Last Modified: Fri, 02 Apr 2021 18:52:23 GMT  
		Size: 1.2 MB (1221589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee602665c1713065c6eead979fd462f942b7d7189161df8168b23a4ab5c5c1b0`  
		Last Modified: Fri, 02 Apr 2021 18:52:23 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:73bbbb1238c100177fb2bc24bcac1b599c45de279d9b0c5c8b73869b1b36db0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111181631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98212955f480b1c834167f05d6221b7340f518364424ce63e375263e343b4613`
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
# Fri, 02 Apr 2021 00:09:57 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:52:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:52:49 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:53:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:53:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:54:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:40:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:40:08 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 19:02:27 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 19:02:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 19:02:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 19:03:19 GMT
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
	-	`sha256:de79052905e4120d804a4aac99d4f39ba3e122ac3c75efe8363ad5adf256f927`  
		Last Modified: Fri, 02 Apr 2021 01:43:50 GMT  
		Size: 101.7 MB (101698695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c365eb52b58a9023f2a7c4766d48472e0a447c37c43cb6ad323f2cc8d6c1c`  
		Last Modified: Fri, 02 Apr 2021 01:42:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6214666ea97e54cb4b48c6e316c3542dd3cdee7f0473e72572c8bc3eacea93`  
		Last Modified: Fri, 02 Apr 2021 03:40:56 GMT  
		Size: 5.6 MB (5558125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9e094ef99cac0175242d7df4a1381918a7c602cc591dbf623d401e1fb1a711`  
		Last Modified: Fri, 02 Apr 2021 19:05:30 GMT  
		Size: 1.2 MB (1219458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40c204ad1fccd1c6eb4773005a7f7219ec24d3926ffef501f6adcceeefbc61b`  
		Last Modified: Fri, 02 Apr 2021 19:05:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:08eaf7a5776da557c1db6c274e87475695fa4698d7b43c7940b8bbecf247915a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111710773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a97900c49d5b44c8c352da00af28fec5f19dcd3788e7612931c0c0a2f57bc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:36:18 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:36:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:36:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:44:23 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:48:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:49:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:37 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:39:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:39:18 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:48:03 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:48:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:48:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:48:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:48:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d3c479d6df2bd83adc83bbac78968bfb4e1abcf6fe557f118b9209078d2ad7`  
		Last Modified: Thu, 01 Apr 2021 16:47:42 GMT  
		Size: 281.5 KB (281483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ae0fd282dc382614f6f786d6a0fc72ed7f4b2054371020563e3e69df43b012`  
		Last Modified: Thu, 01 Apr 2021 16:47:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b472b1c93ad35dfad1b4e65e64156f0f44aa1fe7f105a2d55047d5238852`  
		Last Modified: Fri, 02 Apr 2021 01:13:47 GMT  
		Size: 101.0 MB (101041047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8038507963aca0d9a0c18e8e1870c46927fa6301b0b78be430c58c5e396bee2`  
		Last Modified: Fri, 02 Apr 2021 01:13:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17c1acee68686ada56220f5be4f872287caabbc3f1bc839e349bd00fccad975`  
		Last Modified: Fri, 02 Apr 2021 02:40:36 GMT  
		Size: 6.5 MB (6474039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7484fe4a43db2e2499090ce4f4c7c3af60193ba8366a7e562acba334b1fc0322`  
		Last Modified: Fri, 02 Apr 2021 18:49:42 GMT  
		Size: 1.2 MB (1201567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df5e6b067c7995a06f0f74ef2fc94adb9f26adf36db39dfd86f259db453eae`  
		Last Modified: Fri, 02 Apr 2021 18:49:42 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:beafcff354118be6cd1946efd9ca2028d36de418a510abc6c65321c08f116a63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110604319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40416b4b95b5338e9d6917f544078a6208c1f7fb7e2620b32fb40c053a634b1e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:30:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:30:38 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:09:14 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 03:11:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:11:20 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:11:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:11:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:11:51 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:24:35 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:24:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:24:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:24:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:24:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc638e60e2f17921f3b4535edbf7095cc97278ba8d1410fd7e018101a1242be3`  
		Last Modified: Thu, 01 Apr 2021 04:44:03 GMT  
		Size: 283.4 KB (283416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b706ed0ac7a9324a306982c3913517f4f044be650413df529bf27a05c288d1b9`  
		Last Modified: Thu, 01 Apr 2021 04:44:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b169d190e0156b6deab2ff0e58a47150fc50f2868a89d84eb61c9570305e930`  
		Last Modified: Fri, 02 Apr 2021 03:23:03 GMT  
		Size: 99.5 MB (99513251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83adeb4b646f1b8b0b72cac1632f1bddf6a8b5499291eb0fec11957739b98ec1`  
		Last Modified: Fri, 02 Apr 2021 03:22:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604836dc523b402ec6de96489b450d95b267f41ae391d700d4d21b759ffde953`  
		Last Modified: Fri, 02 Apr 2021 05:04:42 GMT  
		Size: 6.8 MB (6823220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4317a229e7753654e9d8b6b11dae3b5cb7be5941f353851b897405e9846c4d56`  
		Last Modified: Fri, 02 Apr 2021 18:25:36 GMT  
		Size: 1.2 MB (1170495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44a0398c5bef844d519cc025aa24a3ebf5343578a6bb8b3632cad3f0842284e`  
		Last Modified: Fri, 02 Apr 2021 18:25:36 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d363d8e70a8277c2cd56a4cdf4c9527b06097d4f7289a9386ce4c8930246bb01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115430971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf585bf0a2c7796ab5124b11aee2e6b61436fb1e98d0061ffc1414e4b77f54d`
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
# Fri, 02 Apr 2021 00:42:03 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:43:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.16.3.src.tar.gz'; 	sha256='b298d29de9236ca47a023e382313bcc2d2eed31dfa706b60a04103ce83a71a25'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:43:36 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:43:37 GMT
WORKDIR /go
# Fri, 02 Apr 2021 18:41:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 18:41:50 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:41:50 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:41:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 18:41:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 18:41:52 GMT
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
	-	`sha256:d84d135a3d538231dcbc75989d5cb96ac1fd2d8aafd066e7d696d295d4252940`  
		Last Modified: Fri, 02 Apr 2021 00:50:10 GMT  
		Size: 104.8 MB (104809692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de86cbaefc9f6a24519f984378bc3ea0033c6767c5cfa28afeb50edc9a86c5f`  
		Last Modified: Fri, 02 Apr 2021 00:49:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65369d0863ca497de787c86268a4c35482ace4570eabbba157106b2895427ed7`  
		Last Modified: Fri, 02 Apr 2021 18:42:22 GMT  
		Size: 6.5 MB (6471846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9682c6a1905e52c629b4a35d0b39e7c2ff1467d4366a479416007c844fdb4fc6`  
		Last Modified: Fri, 02 Apr 2021 18:42:22 GMT  
		Size: 1.3 MB (1264432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f7f3cd797d6b812a051ae4023b788dc562657b43de6f56c3bffc732a702f40`  
		Last Modified: Fri, 02 Apr 2021 18:42:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:05e5bc7c1e9119bf33b65195ab7c34cc5e1f29c2e635cc0adfd7de3dcb51330b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2.4.0-beta.2-builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:9d285ead4bdf8f99fedfbe03501c691819e48f831e0b0084580a59cb8bf0bad4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2641868622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c93dc0b0fa48b343cd322c901f869fc6a46e264b6256d2fec7f4be8f2b219e04`
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
# Fri, 02 Apr 2021 00:15:25 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:18:07 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'a4400345135b36cb7942e52bbaf978b66814738b855eeff8de879a09fd99de7f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:18:09 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 18:22:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:22:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:22:09 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:22:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:22:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 18:22:38 GMT
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
	-	`sha256:9a7e34d0221e19de26b1af5fb6e32ddd3d7af02c7da8f8797c0b1d88608c507e`  
		Last Modified: Fri, 02 Apr 2021 00:36:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7c9e37d4f37ac6c3bbb4a4ea26623159bd41ab01eeb97ba5f3558f6f0b2e6c`  
		Last Modified: Fri, 02 Apr 2021 00:36:59 GMT  
		Size: 143.7 MB (143721828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14239a8d1f9055a3b8d9d966990a90be84c447b26212c8c31746315beb5af592`  
		Last Modified: Fri, 02 Apr 2021 00:36:22 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cf60572a4ce4c53cd6b737d1d0052857aefd64967385c2dfb51ca7ab737d87`  
		Last Modified: Fri, 02 Apr 2021 18:26:11 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb15e0f080d4ffebac67b5651ae2308c376db5d2c6d35645ce7a3df70088d1a`  
		Last Modified: Fri, 02 Apr 2021 18:26:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933d5696db6c53091e2d4ec83ddc685bd4ac95836dc1adc50e05ed712658a869`  
		Last Modified: Fri, 02 Apr 2021 18:26:08 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa8b4229fc77631db90295128b3ee38f226ce9855444819dde0ec638023b873`  
		Last Modified: Fri, 02 Apr 2021 18:26:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42288aa25a7176680ab6a682e44da10f14581942c25ed0cddc0827b54cae0bad`  
		Last Modified: Fri, 02 Apr 2021 18:26:09 GMT  
		Size: 1.7 MB (1714787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284cd2af3a6274b07a526bf01c7021477428137fd0f4938856f2a10d5dc78d0e`  
		Last Modified: Fri, 02 Apr 2021 18:26:12 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:62c5aa2fde38d3dc0b4bdba5d4b8142a001ee2ef8e355243901203318adb8d3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:c1cfba3a3aa32a96fa4d6b325e56473c26a28d6f3db68ba2d8704a3fc1be6c49
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6003045589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79ee0f3301ee81e21e378ce3f53b7305e6e3db4119c6f6bc1e8ab85411402213`
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
# Fri, 02 Apr 2021 00:18:24 GMT
ENV GOLANG_VERSION=1.16.3
# Fri, 02 Apr 2021 00:22:41 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.16.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'a4400345135b36cb7942e52bbaf978b66814738b855eeff8de879a09fd99de7f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:22:43 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 18:22:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:22:46 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 18:22:47 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:22:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 18:24:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 18:24:20 GMT
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
	-	`sha256:5e7c38f99787bf274ac0a56d06ab8d5ada8675bdbc1b8a41ac4e8e005be67cf3`  
		Last Modified: Fri, 02 Apr 2021 00:37:20 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858a80496ac8841bb47d698f77d63b80c5bfb5c71f3e836cd63729731eb2d0c3`  
		Last Modified: Fri, 02 Apr 2021 00:40:16 GMT  
		Size: 149.2 MB (149164836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f6bce455ff0310e2c186805aff8794f0ae69ed9bac6df06f7f6240d1ba4212`  
		Last Modified: Fri, 02 Apr 2021 00:37:20 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6470d57243826b35d3959d11a867738f749a6118e42d9881bae1d6d022b5cd`  
		Last Modified: Fri, 02 Apr 2021 18:26:22 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2dc30f3688f8d90d917c010cffed48167b0a15f018655d85d79ffc5b7522885`  
		Last Modified: Fri, 02 Apr 2021 18:26:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d18daa399267ca08468b3402c46122b9aa3e5e80c7fb1860558585100eca16c`  
		Last Modified: Fri, 02 Apr 2021 18:26:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcedff24a492766afee3560aca62ebae75ec3a54f253d95c44247b79d24b27a`  
		Last Modified: Fri, 02 Apr 2021 18:26:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d328d81e64b61062f2891b3c48b51ccb4badcbe1efc420c2acbfc43938f5d5ef`  
		Last Modified: Fri, 02 Apr 2021 18:26:25 GMT  
		Size: 11.5 MB (11539007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228dc315d7ba3fe405accce7eafdd95cd5861cda759a223fae2852cceaa01213`  
		Last Modified: Fri, 02 Apr 2021 18:26:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-windowsservercore`

```console
$ docker pull caddy@sha256:9317eb58acc4a0bcc3d093e9939e76dd3f8f659360c81654b28449972ceeab55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:6f39355785ee4e6f020cd3755adb37e0f09f396afd9fcaa7330e15d424e225b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487602702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11dbe1305e7cbce4d507512474f6d9c114c88ecf4c1e6ac3802065b47d6c175c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:16:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 02 Apr 2021 18:16:24 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:16:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9f41c88fc8c2c28230c5eb67fb7d9ef23477a351fb716a44486b3d1a37569fb141112cd3582adcd44424b2819c22723fb49023a6d371e1bf8d92eefe4e7e9ed4')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 02 Apr 2021 18:16:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 02 Apr 2021 18:16:56 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 02 Apr 2021 18:16:58 GMT
VOLUME [c:/config]
# Fri, 02 Apr 2021 18:16:59 GMT
VOLUME [c:/data]
# Fri, 02 Apr 2021 18:17:00 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:17:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:17:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:17:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:17:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:17:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:17:09 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:17:10 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:17:11 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:17:29 GMT
RUN caddy version
# Fri, 02 Apr 2021 18:17:30 GMT
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
	-	`sha256:95e2248c328b7b25c2cbbab7676a8e86d131ea6ad52f5f7bd35647a14893a0a2`  
		Last Modified: Fri, 02 Apr 2021 18:25:36 GMT  
		Size: 9.5 MB (9465706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94271d4a9ce601138f36c7f2d749d748b9ced3d0f52764ca356d32860edb5c5`  
		Last Modified: Fri, 02 Apr 2021 18:25:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ca5665516d898633290e493cef794521852475d69230732409986f3ad81705`  
		Last Modified: Fri, 02 Apr 2021 18:25:38 GMT  
		Size: 16.3 MB (16274695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de70870a5fa3de27854447c44c6ba786981cc938c0f362048da4170553463a`  
		Last Modified: Fri, 02 Apr 2021 18:25:32 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3568445127d07f06bf99e10ae664cca603cc31e68c728060dcac8f7e608881`  
		Last Modified: Fri, 02 Apr 2021 18:25:32 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da65ebebad5059d100ae2af112ca25285129bee6131023aa4c8ce7f0f830793a`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48067c5e57f31ce03ffc3422870602c673527153e446f55fe44dc813bebf9b4`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f2e781673fc6a350cf8b08667e71ffdf90d42f5b0a6a1d9da8e29771f1ffc6`  
		Last Modified: Fri, 02 Apr 2021 18:25:29 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8493be2eceb4e6ea31b450a179859bfd185e92ffd3bbf301fcbd9cb409bcb911`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7a94659f6ba05b7478802b8b57b48e51bbc397ddd845b315891c3e32c1be32`  
		Last Modified: Fri, 02 Apr 2021 18:25:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0db2eb1ebe3b7e3abc59d777a66b0b0b8f51cb3378cc265655f1bfcd7e79312`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6c27364edfca6e69e47b72493bac0aa0242ed5630222b468f2511911e9db14`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ed9f38d63bbcecb70291bbc12286363d05cd6e3fb4be3863ea7332dfd32df8`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b92c3fb781472d906952c139a15a924de551954360d972757c2b7fa70127fc7`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc395ee40c1f92ebe4a8630100e8e3a0323cd404b6e2b4a13b8cd01e17514c1`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daab2d67688cedff5bdcbd07535b3be37f2493b23cd92a902e0f241d46be09f`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc8f200f7b9a010feb0546619b1dee830f1b1ec0dc747ad7158ecb0088482c`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd8989a8ea6c4f623b19785b82af238aee316ee6b72e732262a87011c74d62`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d6b1aa36e5bfef2dfa42970c937fc34573ad9f72508693cda371163b8da379`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 302.3 KB (302255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ec29f6e55d821e399842d426dab17fde9d0ddebeb312cbb9e2a7c07cbdf0b3`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-beta.2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:484c688cb48fa269829e7f6b85bc623bc1b5061043c0e673cc323ccb7c465abc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829094060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86b0dff6059a7f821d34de02f7303fd43d1f41212c68037dd2876ebd5663e534`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:19:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 02 Apr 2021 18:19:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9f41c88fc8c2c28230c5eb67fb7d9ef23477a351fb716a44486b3d1a37569fb141112cd3582adcd44424b2819c22723fb49023a6d371e1bf8d92eefe4e7e9ed4')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 02 Apr 2021 18:20:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 02 Apr 2021 18:20:47 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 02 Apr 2021 18:20:48 GMT
VOLUME [c:/config]
# Fri, 02 Apr 2021 18:20:49 GMT
VOLUME [c:/data]
# Fri, 02 Apr 2021 18:20:50 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:20:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:20:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:20:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:20:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:20:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:21:00 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:21:01 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:21:02 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:21:57 GMT
RUN caddy version
# Fri, 02 Apr 2021 18:21:58 GMT
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
	-	`sha256:3839f3b2a37673d4006f18951ce8d65dac9f9e7a60c481cf4fa86898372bcc72`  
		Last Modified: Fri, 02 Apr 2021 18:25:59 GMT  
		Size: 10.2 MB (10196223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35d02bac712107cd6e45e8ecf4c379e9fe8ba144b8b1af73c9fbaeeb9b5ea21`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f861c5228e163fdd027d65ffdb9bf65e90a1940df415ad2c0ce25ab35cd093`  
		Last Modified: Fri, 02 Apr 2021 18:26:01 GMT  
		Size: 21.7 MB (21693316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f4820276b1680a1ec83d16ac48637c3bb3a276c31baaaf17dd757edd9f4188`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d3d58a6632e499c498ca0addf11c2b22067f5427a93e69885d6b38e1b10596`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28b4d2afe9acc4864ab15a603e8672fb2482c1dd648c57e32456bf7765c3c63`  
		Last Modified: Fri, 02 Apr 2021 18:25:53 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6489ff70b21ce91518922c0d1bfd94e89f92403b67f5a24a1825fd37f28f5aaf`  
		Last Modified: Fri, 02 Apr 2021 18:25:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c0ad8640bb2534d11d722e0777eca31ac10db266abae4cbeefcdfc9f1936a8`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7885acef6da7eb82e08e66cab23b2890f3f3dafef9ec189e81f8045c1954afc`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1f28035d278c150033dbc5d05f6fa9dd3ece81bba6b2a85b3453414398f8aa`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19f2df18981d5ee49e3c45183b1d251f5c4ab848c5f6dc0c0816224f900d287`  
		Last Modified: Fri, 02 Apr 2021 18:25:50 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786ed8d22ae84118b965493f2dc3e79c27bb76f8e34470a569d40d5b9197d008`  
		Last Modified: Fri, 02 Apr 2021 18:25:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b1cde58cdb206802bae3748fc1791648ec167a9addfc05d71af8ef80a7263`  
		Last Modified: Fri, 02 Apr 2021 18:25:49 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a08c62e43e038c439e7b271c524bc1b032913ef0a7838c7a28574564267f4d`  
		Last Modified: Fri, 02 Apr 2021 18:25:48 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629328a7926be76a0105b548d269200ac4213b329ac924c6dc34399747a0a6e4`  
		Last Modified: Fri, 02 Apr 2021 18:25:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b6aec700c2791f546afb2dc6d5045b6ea036c6117b574d5ed06454a2eb5e42`  
		Last Modified: Fri, 02 Apr 2021 18:25:47 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ded6ed75772c3a5c3485bda081d2914ed7b8b0850d62e3d9b9dcfcb86b97961`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55d3e22aa51f274d765555ceb7acfe4c95dfdf06ed747cb78ff3955ec37b43a`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1282f41e60a0e981888559572f13a307d872bb4fb6d636ea2af4a71aa953d4`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 268.3 KB (268326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a7b2d83b6c9a47753c8f82981aefe854fefc34fa7f1ee836fd656fc47f38d`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:e7a72a2929cde204c888cc4d457c93dec116ff9429db95a78aebcb5b7cdbce1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:2.4.0-beta.2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:6f39355785ee4e6f020cd3755adb37e0f09f396afd9fcaa7330e15d424e225b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2487602702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11dbe1305e7cbce4d507512474f6d9c114c88ecf4c1e6ac3802065b47d6c175c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:16:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 02 Apr 2021 18:16:24 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:16:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9f41c88fc8c2c28230c5eb67fb7d9ef23477a351fb716a44486b3d1a37569fb141112cd3582adcd44424b2819c22723fb49023a6d371e1bf8d92eefe4e7e9ed4')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 02 Apr 2021 18:16:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 02 Apr 2021 18:16:56 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 02 Apr 2021 18:16:58 GMT
VOLUME [c:/config]
# Fri, 02 Apr 2021 18:16:59 GMT
VOLUME [c:/data]
# Fri, 02 Apr 2021 18:17:00 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:17:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:17:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:17:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:17:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:17:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:17:09 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:17:10 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:17:11 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:17:29 GMT
RUN caddy version
# Fri, 02 Apr 2021 18:17:30 GMT
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
	-	`sha256:95e2248c328b7b25c2cbbab7676a8e86d131ea6ad52f5f7bd35647a14893a0a2`  
		Last Modified: Fri, 02 Apr 2021 18:25:36 GMT  
		Size: 9.5 MB (9465706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94271d4a9ce601138f36c7f2d749d748b9ced3d0f52764ca356d32860edb5c5`  
		Last Modified: Fri, 02 Apr 2021 18:25:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ca5665516d898633290e493cef794521852475d69230732409986f3ad81705`  
		Last Modified: Fri, 02 Apr 2021 18:25:38 GMT  
		Size: 16.3 MB (16274695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de70870a5fa3de27854447c44c6ba786981cc938c0f362048da4170553463a`  
		Last Modified: Fri, 02 Apr 2021 18:25:32 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3568445127d07f06bf99e10ae664cca603cc31e68c728060dcac8f7e608881`  
		Last Modified: Fri, 02 Apr 2021 18:25:32 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da65ebebad5059d100ae2af112ca25285129bee6131023aa4c8ce7f0f830793a`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48067c5e57f31ce03ffc3422870602c673527153e446f55fe44dc813bebf9b4`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f2e781673fc6a350cf8b08667e71ffdf90d42f5b0a6a1d9da8e29771f1ffc6`  
		Last Modified: Fri, 02 Apr 2021 18:25:29 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8493be2eceb4e6ea31b450a179859bfd185e92ffd3bbf301fcbd9cb409bcb911`  
		Last Modified: Fri, 02 Apr 2021 18:25:30 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7a94659f6ba05b7478802b8b57b48e51bbc397ddd845b315891c3e32c1be32`  
		Last Modified: Fri, 02 Apr 2021 18:25:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0db2eb1ebe3b7e3abc59d777a66b0b0b8f51cb3378cc265655f1bfcd7e79312`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6c27364edfca6e69e47b72493bac0aa0242ed5630222b468f2511911e9db14`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ed9f38d63bbcecb70291bbc12286363d05cd6e3fb4be3863ea7332dfd32df8`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b92c3fb781472d906952c139a15a924de551954360d972757c2b7fa70127fc7`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc395ee40c1f92ebe4a8630100e8e3a0323cd404b6e2b4a13b8cd01e17514c1`  
		Last Modified: Fri, 02 Apr 2021 18:25:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daab2d67688cedff5bdcbd07535b3be37f2493b23cd92a902e0f241d46be09f`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc8f200f7b9a010feb0546619b1dee830f1b1ec0dc747ad7158ecb0088482c`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd8989a8ea6c4f623b19785b82af238aee316ee6b72e732262a87011c74d62`  
		Last Modified: Fri, 02 Apr 2021 18:25:24 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d6b1aa36e5bfef2dfa42970c937fc34573ad9f72508693cda371163b8da379`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 302.3 KB (302255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ec29f6e55d821e399842d426dab17fde9d0ddebeb312cbb9e2a7c07cbdf0b3`  
		Last Modified: Fri, 02 Apr 2021 18:25:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-beta.2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f57f6f7a4a29f7e389643b3741a63fdaf1bc7956b10bf4227af552477f5f64cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:2.4.0-beta.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:484c688cb48fa269829e7f6b85bc623bc1b5061043c0e673cc323ccb7c465abc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5829094060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86b0dff6059a7f821d34de02f7303fd43d1f41212c68037dd2876ebd5663e534`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 18:19:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/e784a6dd41d1cd4f72de2a427961bfb097b72cf9/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 02 Apr 2021 18:19:04 GMT
ENV CADDY_VERSION=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0-beta.2/caddy_2.4.0-beta.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9f41c88fc8c2c28230c5eb67fb7d9ef23477a351fb716a44486b3d1a37569fb141112cd3582adcd44424b2819c22723fb49023a6d371e1bf8d92eefe4e7e9ed4')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 02 Apr 2021 18:20:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 02 Apr 2021 18:20:47 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 02 Apr 2021 18:20:48 GMT
VOLUME [c:/config]
# Fri, 02 Apr 2021 18:20:49 GMT
VOLUME [c:/data]
# Fri, 02 Apr 2021 18:20:50 GMT
LABEL org.opencontainers.image.version=v2.4.0-beta.2
# Fri, 02 Apr 2021 18:20:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 02 Apr 2021 18:20:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 02 Apr 2021 18:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 02 Apr 2021 18:20:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 02 Apr 2021 18:20:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 02 Apr 2021 18:20:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 02 Apr 2021 18:20:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 02 Apr 2021 18:21:00 GMT
EXPOSE 80
# Fri, 02 Apr 2021 18:21:01 GMT
EXPOSE 443
# Fri, 02 Apr 2021 18:21:02 GMT
EXPOSE 2019
# Fri, 02 Apr 2021 18:21:57 GMT
RUN caddy version
# Fri, 02 Apr 2021 18:21:58 GMT
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
	-	`sha256:3839f3b2a37673d4006f18951ce8d65dac9f9e7a60c481cf4fa86898372bcc72`  
		Last Modified: Fri, 02 Apr 2021 18:25:59 GMT  
		Size: 10.2 MB (10196223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35d02bac712107cd6e45e8ecf4c379e9fe8ba144b8b1af73c9fbaeeb9b5ea21`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f861c5228e163fdd027d65ffdb9bf65e90a1940df415ad2c0ce25ab35cd093`  
		Last Modified: Fri, 02 Apr 2021 18:26:01 GMT  
		Size: 21.7 MB (21693316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f4820276b1680a1ec83d16ac48637c3bb3a276c31baaaf17dd757edd9f4188`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d3d58a6632e499c498ca0addf11c2b22067f5427a93e69885d6b38e1b10596`  
		Last Modified: Fri, 02 Apr 2021 18:25:54 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28b4d2afe9acc4864ab15a603e8672fb2482c1dd648c57e32456bf7765c3c63`  
		Last Modified: Fri, 02 Apr 2021 18:25:53 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6489ff70b21ce91518922c0d1bfd94e89f92403b67f5a24a1825fd37f28f5aaf`  
		Last Modified: Fri, 02 Apr 2021 18:25:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c0ad8640bb2534d11d722e0777eca31ac10db266abae4cbeefcdfc9f1936a8`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7885acef6da7eb82e08e66cab23b2890f3f3dafef9ec189e81f8045c1954afc`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1f28035d278c150033dbc5d05f6fa9dd3ece81bba6b2a85b3453414398f8aa`  
		Last Modified: Fri, 02 Apr 2021 18:25:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19f2df18981d5ee49e3c45183b1d251f5c4ab848c5f6dc0c0816224f900d287`  
		Last Modified: Fri, 02 Apr 2021 18:25:50 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786ed8d22ae84118b965493f2dc3e79c27bb76f8e34470a569d40d5b9197d008`  
		Last Modified: Fri, 02 Apr 2021 18:25:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b1cde58cdb206802bae3748fc1791648ec167a9addfc05d71af8ef80a7263`  
		Last Modified: Fri, 02 Apr 2021 18:25:49 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a08c62e43e038c439e7b271c524bc1b032913ef0a7838c7a28574564267f4d`  
		Last Modified: Fri, 02 Apr 2021 18:25:48 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629328a7926be76a0105b548d269200ac4213b329ac924c6dc34399747a0a6e4`  
		Last Modified: Fri, 02 Apr 2021 18:25:48 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b6aec700c2791f546afb2dc6d5045b6ea036c6117b574d5ed06454a2eb5e42`  
		Last Modified: Fri, 02 Apr 2021 18:25:47 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ded6ed75772c3a5c3485bda081d2914ed7b8b0850d62e3d9b9dcfcb86b97961`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55d3e22aa51f274d765555ceb7acfe4c95dfdf06ed747cb78ff3955ec37b43a`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1282f41e60a0e981888559572f13a307d872bb4fb6d636ea2af4a71aa953d4`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 268.3 KB (268326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a7b2d83b6c9a47753c8f82981aefe854fefc34fa7f1ee836fd656fc47f38d`  
		Last Modified: Fri, 02 Apr 2021 18:25:46 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:021184a7ff5b69864870d5968152f6b6235acdfeec77821f1e2be79fd0ea08f4
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
$ docker pull caddy@sha256:bffc665d927b1ed51d5f36dafc191678472776dea35931198b09deebbe4d31fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f81a6d1059252f032458e7bf5dff42ef2844beec6f1c212b5901fb867fdf0a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:19:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 20:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 20:19:34 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 20:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 20:20:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 20:20:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 20:20:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 20:20:18 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 20:20:23 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 20:20:31 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 20:20:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 20:20:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 20:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 20:21:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 20:21:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 20:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 20:21:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 20:21:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 20:21:27 GMT
EXPOSE 443
# Thu, 01 Apr 2021 20:21:33 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 20:21:42 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 20:21:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc0e09b51c0cca190757d6fc9c2b15a635a361717a65973c8d6edf77918d6d5`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 302.3 KB (302335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091713ba252aea42d1ddb0424ba2c2861b3afd2d0102c5d0a6070bacd31e8b49`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840f6bc70853fb9cc5e9c5752486488368649459a0beaa0684081a5b4a44bd4`  
		Last Modified: Thu, 01 Apr 2021 20:27:42 GMT  
		Size: 10.2 MB (10241392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb03f086aa28c855432404e128ff2009c1198d61578654e584a12062e24953f`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 153.0 B  
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
$ docker pull caddy@sha256:24e707cb4e7f90c12ca1f5fb4c1df08134db8d1ede9b2bce4075f12176f270b2
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
$ docker pull caddy@sha256:ece02ddc55072c0f8170999a314bae216c7a2e9a9b6848e61a6284a9d73f94f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119528273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b85122de32749bb4ce99c4ec210d0b3f4ae7520aeb96d1b3409d7e164a5419`
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
# Fri, 02 Apr 2021 00:26:55 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:28:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:28:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:28:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:28:39 GMT
WORKDIR /go
# Fri, 02 Apr 2021 00:49:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 00:49:44 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 00:49:45 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 00:49:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 00:49:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 00:49:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 00:49:48 GMT
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
	-	`sha256:7fb06cf977208e0278301057f91233255a165debf7803f76081637b1a3fe2df4`  
		Last Modified: Fri, 02 Apr 2021 00:33:59 GMT  
		Size: 106.8 MB (106825493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d4990aca24e7f5bc780b0b6a54b4ffe9309e35aa07fbc5a0a37e0ea3d9f9ba`  
		Last Modified: Fri, 02 Apr 2021 00:33:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82125fdcb93000a2f7bac7bfb8862942871d32af42e10627aacbd1920dccc98b`  
		Last Modified: Fri, 02 Apr 2021 00:50:30 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24a53b2e0122830bff05a8cf66417dca406c3a78c2c50f57ed18b9eabd310c`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 1.3 MB (1311070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8315f3a639f17e3d2f1c8a9375c23b4449414ba0dcfddb8a5b7706e54ad36ef4`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:10d41528f228b48108732d502adc636fca65043411bc0f7290dd76c8edd037cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114712667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:025a88409e4f77fb03240b210876fca131968a56bded41bc910094fed80cf415`
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
# Fri, 02 Apr 2021 01:30:32 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:33:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:33:22 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:33:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:33:34 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:09:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:09:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:09:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:09:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:09:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:09:09 GMT
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
	-	`sha256:4091fa2dc5e0d5be46942830e27d3a5f436a9cb7f46dcc3c113da4dbcbea3040`  
		Last Modified: Fri, 02 Apr 2021 01:39:32 GMT  
		Size: 102.7 MB (102675361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be92ead41aa69a067ce5cb63f8e52a4437d23028ba34a3278d8dd25fefb2fca`  
		Last Modified: Fri, 02 Apr 2021 01:38:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0149c588c89df3be653be7fd1e1adfd8a1294acdf6b72e7389cf0974752985`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 7.9 MB (7929365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e0d86690298b1f2e60ba7793d37b00c6110c464eea7b3f3f55d666976fc4b`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd374a07a01a50e87ff86e4e2aed8910bea99eaa7f85a92e48cddef6ce1695e2`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:055b54c865e8f858fb4592a56a49eccad632fd9d67a45161586e716a68de125c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5ae4a80046d3819c7c459fcdbbb9885b9550347e3ae2d08bf36c6b56ddb901`
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
# Fri, 02 Apr 2021 01:33:58 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:38:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:38:43 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:38:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:38:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:38:54 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:39:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:39:48 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:39:49 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:39:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:39:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:39:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:39:54 GMT
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
	-	`sha256:246e9d6efa3b5ddb94ed08d2c44063063809626f1b8945ab7fd8f608c27b612c`  
		Last Modified: Fri, 02 Apr 2021 01:49:28 GMT  
		Size: 102.5 MB (102462038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185aeca957b64890215aa6243b0ed41133921755346cb5630f47811efe98d924`  
		Last Modified: Fri, 02 Apr 2021 01:48:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561958899ceda559293617ab883e3c7c50ec0d82c29b163b971862b589f19fd7`  
		Last Modified: Fri, 02 Apr 2021 03:40:46 GMT  
		Size: 7.1 MB (7145600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0c3c642c83a6e2e01f091cfa2000f1edd689ea6d1ca5d6fd073c13e795c20`  
		Last Modified: Fri, 02 Apr 2021 03:40:43 GMT  
		Size: 1.2 MB (1219444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d966c9600d6d83b44c77316d87064bcb298ef3c6cc8a488b66eb658be3d31f`  
		Last Modified: Fri, 02 Apr 2021 03:40:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:68996d8d9053274f585d31e72a5606c5b8efc0c22715a722efcb184769dfeb62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114829795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680177f28f49f5cc8e4add6e48c3cf149cc27044bd36825e3ebc2be149c33d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:39:14 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:39:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:04:26 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:07:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:07:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:08:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:08:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:08:57 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:38:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:38:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:38:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:38:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:38:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:38:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:38:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad1fe544e25b6d321ae8fdcd682a086ba01b0cb7a6156e4b56678c814e705a9`  
		Last Modified: Thu, 01 Apr 2021 16:48:38 GMT  
		Size: 281.2 KB (281223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4362df3d97a48df3f56e407e87e3bb4b9ff06e2b28fe3c6b5d9efc43c603c3ea`  
		Last Modified: Thu, 01 Apr 2021 16:48:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf580103e01a743f2033316ab60816b69e6a6d3cc87bd05d4d5e3c01753b59a`  
		Last Modified: Fri, 02 Apr 2021 01:17:28 GMT  
		Size: 102.1 MB (102136450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d59c655ea056d2547111351a9f74cbb1760fd590e7b4d9daf1a3adefabc47`  
		Last Modified: Fri, 02 Apr 2021 01:17:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf4373967e0c510b0e8a50f6a81c276fb4ec40854edffdef61a4101ddcc2d0`  
		Last Modified: Fri, 02 Apr 2021 02:40:20 GMT  
		Size: 8.5 MB (8500007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f4ba979d45ec198f862cb4c75488f29795eeb8706732280704829c8eebb2c`  
		Last Modified: Fri, 02 Apr 2021 02:40:18 GMT  
		Size: 1.2 MB (1201548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ba1a31428dd993c50efd22bf7b473e3505752416376f8d60b61682011823a`  
		Last Modified: Fri, 02 Apr 2021 02:40:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:b4d7764de3f8d29cbb22b2b973802bbf36aa89b6c1e6a11cf6934b2273b80e59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113988669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c777710e48b168e93b792b4171e667a5c16209c668b09dd54d442ad4ef1c55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:33:46 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:33:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:33:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:18:36 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 03:20:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:20:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:20:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:21:02 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:11 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 05:03:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 05:03:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 05:03:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 05:03:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 05:03:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ce9f93b1dd5f42d7663646400f1307cddfad6a5361031e3a1ca8c46d90d2e`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 283.2 KB (283224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb52babc5b3ae7ccfca63bfc4092e7d57cbd51bc203af266e4fcb0169a6107`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91ebeddf57ad09e8e1b3eb1e312be6a4484d88f8f970a7b241d759abe98e5f`  
		Last Modified: Fri, 02 Apr 2021 03:25:31 GMT  
		Size: 100.8 MB (100806744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac05f37b09f2517038025dd2d905a5d3ecbd9af697023fe05bc857ed48b8f455`  
		Last Modified: Fri, 02 Apr 2021 03:25:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e2e6a908474ce0f09d3cc2e30293784024f2a821c330690e753b01155c5346`  
		Last Modified: Fri, 02 Apr 2021 05:04:26 GMT  
		Size: 8.9 MB (8921423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b888e7962a16510b476660b91df0be664af7f16e7eb94288112b51bfd206995`  
		Last Modified: Fri, 02 Apr 2021 05:04:25 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ce4e5965570ab285f5e3be6ab2ca4cd6b618b344303a3e09cbb4c46fb2393f`  
		Last Modified: Fri, 02 Apr 2021 05:04:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:55343bb8a3d3c8060510dda018530e00e140b628136dd4d2e80d5235d9f81310
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118407979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5002b31cde12b4652640e74c39b0c4f6e71cf200aebef971c3dc23634cb9d859`
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
# Fri, 02 Apr 2021 00:47:37 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:48:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:59 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:48:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:59:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:59:07 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:59:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:59:09 GMT
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
	-	`sha256:665e4b76c3c27678347c855f22a12fc05bfe995765d883647a9c2441b9b069d0`  
		Last Modified: Fri, 02 Apr 2021 00:52:06 GMT  
		Size: 105.9 MB (105941238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00e4cb90e6507b991c002adcd7422fee334b80a8f1e5ac783562c6be88675a3`  
		Last Modified: Fri, 02 Apr 2021 00:51:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8845c8ed835494d2be5205c635b53fd5ab4b00d5d26a3334e616c5b014bb0d`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 8.4 MB (8352795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bdec70ad8c727647ea8e85bfee6409d5f5c98958898ba25b0b2fcb779e76fa`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 1.3 MB (1264423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4492bd0a1a8e714b581c18713607112324a6401040484d4ef05de25a16d89`  
		Last Modified: Fri, 02 Apr 2021 02:59:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:89576372020fc2eb4c0a7f3a3e1202a7b5833822dcac78836f6f48dc05cf1b15
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636681347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433619fcb10b7d636ff7d2ab6165f3648a45f1587bf0fc5a17c16bb0b4ea13f9`
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
# Fri, 02 Apr 2021 00:25:42 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:23 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:28:25 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:03:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:03:35 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:03:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:03:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:04:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:04:05 GMT
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
	-	`sha256:ddf005729e9b7c9f2912ff8e30bec3d383755302fe0b20e361d87ed43a703519`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9af25c23d2108f315f14a45d27ecfe24ceb05852132cf721a61ee44495e1a`  
		Last Modified: Fri, 02 Apr 2021 00:44:11 GMT  
		Size: 138.5 MB (138534624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1592b7415bb7c21ec31f9b97bed86b4b01c96621f385d9da5903fa7c320d4e47`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae6b99eb587e6a00f40f4c134c6b7d4b8d1bc9d9d17b14538d30b6c689e5bc2`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d285524127fff971c8f6c086256b3907c8428d162347bcba0f3bcf6d64fa9`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22f3dc30fb1b76d85e47461eb558cc38cd60ccd8d02c6d8bd9aea7cce3e909`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5063c8d06382902b304af0538c9114e087db04e693551e92d15ffd12dcca542`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313a2e87390c3ef15da4fd9f3b978ef539bc6b5bf8d3e54d23f28e4acd386563`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.7 MB (1715051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ed62f1fbb34e8dfbbf3e11e5f7aa91c4e21c7ac1debbbf86e2561d6ecc5ea`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:017255652cc26ea2af428ecc3b6f2222ee64d88cfdf1c34e3522f048aa461ee9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997836720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a9fde1e66982a65a46dea5c07548ac8afcd29b6f304afe23a8ea9bcdcf186f`
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
# Fri, 02 Apr 2021 00:28:41 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:32:35 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:32:37 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:04:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:04:14 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:04:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:04:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:05:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:05:45 GMT
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
	-	`sha256:a055a610a3b2e63b54d561bc3512bd068b4443a7417486b9dc65a4ad292583c7`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c202a262d335726e6d079774ca9e11f52da7326ee18860265595a97527a7b545`  
		Last Modified: Fri, 02 Apr 2021 00:44:55 GMT  
		Size: 144.0 MB (143966864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737da401effa5536406d2508db65af6f54d9be0a3c5f1347ae56dc5ad1b8c1a4`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.6 KB (1579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c52d85af463d5a66468c058122750336a2d002544c19dbaff721875cb8c6c24`  
		Last Modified: Fri, 02 Apr 2021 01:09:48 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f1bf71cbf1adab82ad5a9d8f5b71571306bf6bcf254b686963f2ed7562e7fc`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba22c0fd4b07e8d5ff2ab18028eb3f4d87c20420e43a2afbf78c8da9032399b2`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b238ffe2f30d1bebcac0de5c7d019504926664c08f5730389c7c1e426c12a`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0b00fc7a9cc9546977571c1922da63009fc89865ee5ae6b603cdf38d5b56ad`  
		Last Modified: Fri, 02 Apr 2021 01:09:47 GMT  
		Size: 11.5 MB (11528518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606193453afd7f6b2c5d21cdd640e297c0e3b0514642cc7044ff5a83ef6e66c7`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:7d7b5f18ee38ce53f1af5300bf9d3e4297def83236cbe1769bc50cf631048fa5
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
$ docker pull caddy@sha256:ece02ddc55072c0f8170999a314bae216c7a2e9a9b6848e61a6284a9d73f94f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119528273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b85122de32749bb4ce99c4ec210d0b3f4ae7520aeb96d1b3409d7e164a5419`
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
# Fri, 02 Apr 2021 00:26:55 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:28:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:28:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:28:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:28:39 GMT
WORKDIR /go
# Fri, 02 Apr 2021 00:49:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 00:49:44 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 00:49:45 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 00:49:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 00:49:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 00:49:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 00:49:48 GMT
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
	-	`sha256:7fb06cf977208e0278301057f91233255a165debf7803f76081637b1a3fe2df4`  
		Last Modified: Fri, 02 Apr 2021 00:33:59 GMT  
		Size: 106.8 MB (106825493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d4990aca24e7f5bc780b0b6a54b4ffe9309e35aa07fbc5a0a37e0ea3d9f9ba`  
		Last Modified: Fri, 02 Apr 2021 00:33:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82125fdcb93000a2f7bac7bfb8862942871d32af42e10627aacbd1920dccc98b`  
		Last Modified: Fri, 02 Apr 2021 00:50:30 GMT  
		Size: 8.3 MB (8310402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24a53b2e0122830bff05a8cf66417dca406c3a78c2c50f57ed18b9eabd310c`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 1.3 MB (1311070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8315f3a639f17e3d2f1c8a9375c23b4449414ba0dcfddb8a5b7706e54ad36ef4`  
		Last Modified: Fri, 02 Apr 2021 00:50:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:10d41528f228b48108732d502adc636fca65043411bc0f7290dd76c8edd037cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114712667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:025a88409e4f77fb03240b210876fca131968a56bded41bc910094fed80cf415`
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
# Fri, 02 Apr 2021 01:30:32 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:33:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:33:22 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:33:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:33:34 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:09:02 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:09:03 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:09:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:09:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:09:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:09:09 GMT
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
	-	`sha256:4091fa2dc5e0d5be46942830e27d3a5f436a9cb7f46dcc3c113da4dbcbea3040`  
		Last Modified: Fri, 02 Apr 2021 01:39:32 GMT  
		Size: 102.7 MB (102675361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be92ead41aa69a067ce5cb63f8e52a4437d23028ba34a3278d8dd25fefb2fca`  
		Last Modified: Fri, 02 Apr 2021 01:38:30 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0149c588c89df3be653be7fd1e1adfd8a1294acdf6b72e7389cf0974752985`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 7.9 MB (7929365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e0d86690298b1f2e60ba7793d37b00c6110c464eea7b3f3f55d666976fc4b`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 1.2 MB (1221590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd374a07a01a50e87ff86e4e2aed8910bea99eaa7f85a92e48cddef6ce1695e2`  
		Last Modified: Fri, 02 Apr 2021 03:10:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:055b54c865e8f858fb4592a56a49eccad632fd9d67a45161586e716a68de125c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113516140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5ae4a80046d3819c7c459fcdbbb9885b9550347e3ae2d08bf36c6b56ddb901`
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
# Fri, 02 Apr 2021 01:33:58 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:38:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:38:43 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:38:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:38:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:38:54 GMT
WORKDIR /go
# Fri, 02 Apr 2021 03:39:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 03:39:48 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 03:39:49 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 03:39:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 03:39:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 03:39:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 03:39:54 GMT
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
	-	`sha256:246e9d6efa3b5ddb94ed08d2c44063063809626f1b8945ab7fd8f608c27b612c`  
		Last Modified: Fri, 02 Apr 2021 01:49:28 GMT  
		Size: 102.5 MB (102462038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185aeca957b64890215aa6243b0ed41133921755346cb5630f47811efe98d924`  
		Last Modified: Fri, 02 Apr 2021 01:48:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561958899ceda559293617ab883e3c7c50ec0d82c29b163b971862b589f19fd7`  
		Last Modified: Fri, 02 Apr 2021 03:40:46 GMT  
		Size: 7.1 MB (7145600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a0c3c642c83a6e2e01f091cfa2000f1edd689ea6d1ca5d6fd073c13e795c20`  
		Last Modified: Fri, 02 Apr 2021 03:40:43 GMT  
		Size: 1.2 MB (1219444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d966c9600d6d83b44c77316d87064bcb298ef3c6cc8a488b66eb658be3d31f`  
		Last Modified: Fri, 02 Apr 2021 03:40:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:68996d8d9053274f585d31e72a5606c5b8efc0c22715a722efcb184769dfeb62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114829795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f680177f28f49f5cc8e4add6e48c3cf149cc27044bd36825e3ebc2be149c33d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:39:14 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 16:39:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 16:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:04:26 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 01:07:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 01:07:54 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 01:08:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 01:08:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 01:08:57 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:38:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:38:38 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:38:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:38:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:38:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:38:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:38:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad1fe544e25b6d321ae8fdcd682a086ba01b0cb7a6156e4b56678c814e705a9`  
		Last Modified: Thu, 01 Apr 2021 16:48:38 GMT  
		Size: 281.2 KB (281223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4362df3d97a48df3f56e407e87e3bb4b9ff06e2b28fe3c6b5d9efc43c603c3ea`  
		Last Modified: Thu, 01 Apr 2021 16:48:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf580103e01a743f2033316ab60816b69e6a6d3cc87bd05d4d5e3c01753b59a`  
		Last Modified: Fri, 02 Apr 2021 01:17:28 GMT  
		Size: 102.1 MB (102136450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0d59c655ea056d2547111351a9f74cbb1760fd590e7b4d9daf1a3adefabc47`  
		Last Modified: Fri, 02 Apr 2021 01:17:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf4373967e0c510b0e8a50f6a81c276fb4ec40854edffdef61a4101ddcc2d0`  
		Last Modified: Fri, 02 Apr 2021 02:40:20 GMT  
		Size: 8.5 MB (8500007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f4ba979d45ec198f862cb4c75488f29795eeb8706732280704829c8eebb2c`  
		Last Modified: Fri, 02 Apr 2021 02:40:18 GMT  
		Size: 1.2 MB (1201548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936ba1a31428dd993c50efd22bf7b473e3505752416376f8d60b61682011823a`  
		Last Modified: Fri, 02 Apr 2021 02:40:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b4d7764de3f8d29cbb22b2b973802bbf36aa89b6c1e6a11cf6934b2273b80e59
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113988669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c777710e48b168e93b792b4171e667a5c16209c668b09dd54d442ad4ef1c55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 04:33:46 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 01 Apr 2021 04:33:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 04:33:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:18:36 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 03:20:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 03:20:38 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 03:20:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 03:20:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 03:21:02 GMT
WORKDIR /go
# Fri, 02 Apr 2021 05:03:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 05:03:11 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 05:03:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 05:03:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 05:03:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 05:03:24 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 05:03:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ce9f93b1dd5f42d7663646400f1307cddfad6a5361031e3a1ca8c46d90d2e`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 283.2 KB (283224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb52babc5b3ae7ccfca63bfc4092e7d57cbd51bc203af266e4fcb0169a6107`  
		Last Modified: Thu, 01 Apr 2021 04:44:51 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd91ebeddf57ad09e8e1b3eb1e312be6a4484d88f8f970a7b241d759abe98e5f`  
		Last Modified: Fri, 02 Apr 2021 03:25:31 GMT  
		Size: 100.8 MB (100806744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac05f37b09f2517038025dd2d905a5d3ecbd9af697023fe05bc857ed48b8f455`  
		Last Modified: Fri, 02 Apr 2021 03:25:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e2e6a908474ce0f09d3cc2e30293784024f2a821c330690e753b01155c5346`  
		Last Modified: Fri, 02 Apr 2021 05:04:26 GMT  
		Size: 8.9 MB (8921423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b888e7962a16510b476660b91df0be664af7f16e7eb94288112b51bfd206995`  
		Last Modified: Fri, 02 Apr 2021 05:04:25 GMT  
		Size: 1.2 MB (1170492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ce4e5965570ab285f5e3be6ab2ca4cd6b618b344303a3e09cbb4c46fb2393f`  
		Last Modified: Fri, 02 Apr 2021 05:04:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:55343bb8a3d3c8060510dda018530e00e140b628136dd4d2e80d5235d9f81310
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118407979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5002b31cde12b4652640e74c39b0c4f6e71cf200aebef971c3dc23634cb9d859`
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
# Fri, 02 Apr 2021 00:47:37 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:48:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.11.src.tar.gz'; 	sha256='f25b2441d4c76cf63cde94d59bab237cc33e8a2a139040d904c8630f46d061e5'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 02 Apr 2021 00:48:59 GMT
ENV GOPATH=/go
# Fri, 02 Apr 2021 00:48:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Apr 2021 00:49:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 02 Apr 2021 00:49:00 GMT
WORKDIR /go
# Fri, 02 Apr 2021 02:59:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 02:59:07 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 02:59:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 02:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='6760a7816d01da49cc6f0e8a476c3e7bd7d3778628b4ddd7edbb69b83fd1d9c086fa51e4195d928526d323f37a52b46a02a62f1ad63fdb511aeec41b83eff7a9' ;; 		armhf)   binArch='armv6'; checksum='9825e195c1abdca6f143d99feb667f8c15181b8dc67e18156c253708e47882cdc4cfffc32b3667f6bfdb2556410136ee11b3df7edca2a7de503f5a4871b0305e' ;; 		armv7)   binArch='armv7'; checksum='9d80d4d1e21135c55ab22a73ee8b45b94aa128c9ef2a95646fff76159ef0087be91641b805f5ea6aea6e949bb197cb051642c3cbf39431f080d70aec55c68854' ;; 		aarch64) binArch='arm64'; checksum='2de63a8305ef485d7cdf5f28f1ca2b68a1f16f051c53035466666d930074aa3be5d32fa69668435cd9dbc9dc84f6fd78307f92caeb4aa544d0032a66bd71514a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='a70446270c35da12ea214072b4f7f9a9d4b59c7ef391e6b2e72cf7a9dab5df1e9eb8d81abed066c5d5036d0a7f5730118ad3b4428df1e0d001b8faf228d368ed' ;; 		s390x)   binArch='s390x'; checksum='b1c72f77caa5bba89b30ef752dc88bd7796975a0a17298fbcc22ddd61ca9d7b1c7aca6b8b9aa231091aea122f9931022552ffe16fc84ebfb9ba936bf53d32367' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 02 Apr 2021 02:59:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 02 Apr 2021 02:59:09 GMT
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
	-	`sha256:665e4b76c3c27678347c855f22a12fc05bfe995765d883647a9c2441b9b069d0`  
		Last Modified: Fri, 02 Apr 2021 00:52:06 GMT  
		Size: 105.9 MB (105941238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00e4cb90e6507b991c002adcd7422fee334b80a8f1e5ac783562c6be88675a3`  
		Last Modified: Fri, 02 Apr 2021 00:51:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8845c8ed835494d2be5205c635b53fd5ab4b00d5d26a3334e616c5b014bb0d`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 8.4 MB (8352795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bdec70ad8c727647ea8e85bfee6409d5f5c98958898ba25b0b2fcb779e76fa`  
		Last Modified: Fri, 02 Apr 2021 02:59:49 GMT  
		Size: 1.3 MB (1264423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4492bd0a1a8e714b581c18713607112324a6401040484d4ef05de25a16d89`  
		Last Modified: Fri, 02 Apr 2021 02:59:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:0c67e10ec967bbb5febbb8307b0e4a234df003c616262fde938f75631cacd2e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull caddy@sha256:89576372020fc2eb4c0a7f3a3e1202a7b5833822dcac78836f6f48dc05cf1b15
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2636681347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433619fcb10b7d636ff7d2ab6165f3648a45f1587bf0fc5a17c16bb0b4ea13f9`
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
# Fri, 02 Apr 2021 00:25:42 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:28:23 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:28:25 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:03:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:03:35 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:03:36 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:03:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:04:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:04:05 GMT
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
	-	`sha256:ddf005729e9b7c9f2912ff8e30bec3d383755302fe0b20e361d87ed43a703519`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9af25c23d2108f315f14a45d27ecfe24ceb05852132cf721a61ee44495e1a`  
		Last Modified: Fri, 02 Apr 2021 00:44:11 GMT  
		Size: 138.5 MB (138534624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1592b7415bb7c21ec31f9b97bed86b4b01c96621f385d9da5903fa7c320d4e47`  
		Last Modified: Fri, 02 Apr 2021 00:43:41 GMT  
		Size: 1.6 KB (1590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae6b99eb587e6a00f40f4c134c6b7d4b8d1bc9d9d17b14538d30b6c689e5bc2`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d285524127fff971c8f6c086256b3907c8428d162347bcba0f3bcf6d64fa9`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22f3dc30fb1b76d85e47461eb558cc38cd60ccd8d02c6d8bd9aea7cce3e909`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5063c8d06382902b304af0538c9114e087db04e693551e92d15ffd12dcca542`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313a2e87390c3ef15da4fd9f3b978ef539bc6b5bf8d3e54d23f28e4acd386563`  
		Last Modified: Fri, 02 Apr 2021 01:09:29 GMT  
		Size: 1.7 MB (1715051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4ed62f1fbb34e8dfbbf3e11e5f7aa91c4e21c7ac1debbbf86e2561d6ecc5ea`  
		Last Modified: Fri, 02 Apr 2021 01:09:26 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:707fee0b94dcb8bb07e1cc0f86e10c540509ee572b69240bc0556cfafa586cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull caddy@sha256:017255652cc26ea2af428ecc3b6f2222ee64d88cfdf1c34e3522f048aa461ee9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997836720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a9fde1e66982a65a46dea5c07548ac8afcd29b6f304afe23a8ea9bcdcf186f`
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
# Fri, 02 Apr 2021 00:28:41 GMT
ENV GOLANG_VERSION=1.15.11
# Fri, 02 Apr 2021 00:32:35 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.11.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '56f63de17cd739287de6d9f3cfdad3b781ad3e4a18aae20ece994ee97c1819fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Fri, 02 Apr 2021 00:32:37 GMT
WORKDIR C:\gopath
# Fri, 02 Apr 2021 01:04:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Apr 2021 01:04:14 GMT
ENV XCADDY_VERSION=v0.1.8
# Fri, 02 Apr 2021 01:04:15 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 02 Apr 2021 01:04:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 02 Apr 2021 01:05:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.8/xcaddy_0.1.8_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('ccbc594da07adff41098959a78efaaee42fca4e5feb7806661d00841229b20ff1c47fed024c7a84e8554d3e8be3f162d3750e5e8347d6a230c496d4b133213e8')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 02 Apr 2021 01:05:45 GMT
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
	-	`sha256:a055a610a3b2e63b54d561bc3512bd068b4443a7417486b9dc65a4ad292583c7`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c202a262d335726e6d079774ca9e11f52da7326ee18860265595a97527a7b545`  
		Last Modified: Fri, 02 Apr 2021 00:44:55 GMT  
		Size: 144.0 MB (143966864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737da401effa5536406d2508db65af6f54d9be0a3c5f1347ae56dc5ad1b8c1a4`  
		Last Modified: Fri, 02 Apr 2021 00:44:26 GMT  
		Size: 1.6 KB (1579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c52d85af463d5a66468c058122750336a2d002544c19dbaff721875cb8c6c24`  
		Last Modified: Fri, 02 Apr 2021 01:09:48 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f1bf71cbf1adab82ad5a9d8f5b71571306bf6bcf254b686963f2ed7562e7fc`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba22c0fd4b07e8d5ff2ab18028eb3f4d87c20420e43a2afbf78c8da9032399b2`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562b238ffe2f30d1bebcac0de5c7d019504926664c08f5730389c7c1e426c12a`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0b00fc7a9cc9546977571c1922da63009fc89865ee5ae6b603cdf38d5b56ad`  
		Last Modified: Fri, 02 Apr 2021 01:09:47 GMT  
		Size: 11.5 MB (11528518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606193453afd7f6b2c5d21cdd640e297c0e3b0514642cc7044ff5a83ef6e66c7`  
		Last Modified: Fri, 02 Apr 2021 01:09:44 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:f9203a727530897ed215241d9cc3f9ca634445f84eabde0197fd53f5d1e00b0a
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
$ docker pull caddy@sha256:bffc665d927b1ed51d5f36dafc191678472776dea35931198b09deebbe4d31fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f81a6d1059252f032458e7bf5dff42ef2844beec6f1c212b5901fb867fdf0a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 20:19:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 01 Apr 2021 20:19:27 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 01 Apr 2021 20:19:34 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 01 Apr 2021 20:19:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 01 Apr 2021 20:20:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 20:20:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 01 Apr 2021 20:20:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 01 Apr 2021 20:20:18 GMT
VOLUME [/config]
# Thu, 01 Apr 2021 20:20:23 GMT
VOLUME [/data]
# Thu, 01 Apr 2021 20:20:31 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 01 Apr 2021 20:20:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 01 Apr 2021 20:20:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 01 Apr 2021 20:20:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 01 Apr 2021 20:21:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 01 Apr 2021 20:21:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 01 Apr 2021 20:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 01 Apr 2021 20:21:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 01 Apr 2021 20:21:21 GMT
EXPOSE 80
# Thu, 01 Apr 2021 20:21:27 GMT
EXPOSE 443
# Thu, 01 Apr 2021 20:21:33 GMT
EXPOSE 2019
# Thu, 01 Apr 2021 20:21:42 GMT
WORKDIR /srv
# Thu, 01 Apr 2021 20:21:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc0e09b51c0cca190757d6fc9c2b15a635a361717a65973c8d6edf77918d6d5`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 302.3 KB (302335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091713ba252aea42d1ddb0424ba2c2861b3afd2d0102c5d0a6070bacd31e8b49`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840f6bc70853fb9cc5e9c5752486488368649459a0beaa0684081a5b4a44bd4`  
		Last Modified: Thu, 01 Apr 2021 20:27:42 GMT  
		Size: 10.2 MB (10241392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb03f086aa28c855432404e128ff2009c1198d61578654e584a12062e24953f`  
		Last Modified: Thu, 01 Apr 2021 20:27:39 GMT  
		Size: 153.0 B  
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
