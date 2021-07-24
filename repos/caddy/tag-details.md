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
-	[`caddy:2.4.3`](#caddy243)
-	[`caddy:2.4.3-alpine`](#caddy243-alpine)
-	[`caddy:2.4.3-builder`](#caddy243-builder)
-	[`caddy:2.4.3-builder-alpine`](#caddy243-builder-alpine)
-	[`caddy:2.4.3-builder-windowsservercore-1809`](#caddy243-builder-windowsservercore-1809)
-	[`caddy:2.4.3-builder-windowsservercore-ltsc2016`](#caddy243-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.3-windowsservercore`](#caddy243-windowsservercore)
-	[`caddy:2.4.3-windowsservercore-1809`](#caddy243-windowsservercore-1809)
-	[`caddy:2.4.3-windowsservercore-ltsc2016`](#caddy243-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:90dfeaa3846391a67e0e9dec49fbe8c3031eec18cdbb92258b2e45bcd1c775d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:77f27025e0e1e0ab97bc931db61d24f9ac41591e17576ab46c4b508afbccacd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14648199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8a741f4852592d8634aa37c7f351ae4f4e7b4a9a2594df54603ac48cbdad74`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 19:19:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 19:19:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 19:19:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 19:19:32 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 19:19:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 443
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 19:19:34 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 19:19:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d589bc046eca71df600301462981053bf178fcd31d4b2c882ca05aec70bacd`  
		Last Modified: Thu, 24 Jun 2021 19:19:59 GMT  
		Size: 11.5 MB (11529821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8ce9421f330c9a085ac8f059d2dd53feabf795c461d4f43b596d0302b1cf9`  
		Last Modified: Thu, 24 Jun 2021 19:19:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:276a06d4fac1a2986e5cade46d37a49e0954fb38a3b5ba846293c68ceef54d58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13816591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e555ad7d2e3449d758dae401706b4cc380e9747165f31c57760faa52fb6174a3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 18:50:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 24 Jun 2021 18:50:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:50:24 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:50:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:50:30 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:50:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:50:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:50:34 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:50:36 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:50:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e861f8792ad39fcefd1d13a12171eb53b6c830fc9182b96acb8bfb97c770fe4`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 300.5 KB (300519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd197178893bbfb4025a2b9c5edf60d3cd30075037c42b24c7b2b31bb8e559`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a2958808e8ef8313c312955baf1311cd2c15671f9d1ca3f59b720bd3c03ad`  
		Last Modified: Thu, 24 Jun 2021 18:52:04 GMT  
		Size: 10.9 MB (10887935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902e2228deaccfd2eec0d2ed45f03d38e9a341e018d1bacff231874d0b8b051`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:975e2acc21fa69679cd59786b1ecd7cf3d8f4ac40b028d61c219fd4e770d14cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88d5f2ec732bdfe5c5785fb90e7258f29e158c1857de067fb62436a723ec081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 04:25:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Jun 2021 04:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Fri, 25 Jun 2021 04:25:57 GMT
ENV CADDY_VERSION=v2.4.3
# Fri, 25 Jun 2021 04:26:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Jun 2021 04:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/config]
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/data]
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Jun 2021 04:26:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 80
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 443
# Fri, 25 Jun 2021 04:26:09 GMT
EXPOSE 2019
# Fri, 25 Jun 2021 04:26:09 GMT
WORKDIR /srv
# Fri, 25 Jun 2021 04:26:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532875903768e2aaa022f0dcc8d36d882e8a7af7edf14e86e6444c2406af868e`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 299.7 KB (299661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141d604c45916aa77667e44622bc085ab97eec4f8ba487d6f06aed74e53395a4`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e46c35d91cdc127af615f56a9074bd03baf63f40550c10ac1e56edf111fd4e`  
		Last Modified: Fri, 25 Jun 2021 04:27:42 GMT  
		Size: 10.9 MB (10863654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7106f92e86cc0f43d86170e3424675fb1543f58df755ce212946b44d5c96c38`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:780ee1b9ce06277bd5c34b2d9a6908cdb3028aa838fa75e5c6e1e32d2cabb417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13464756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a697a3b5305c041fd956ba80c8845676041e98bce128a69e70074e5abe9653dd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:39:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:39:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:39:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:39:33 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:39:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75403ccf5c23126b5dca334871ec0096a90d0fb85f47be1ecba3904921529c0`  
		Last Modified: Thu, 24 Jun 2021 18:40:18 GMT  
		Size: 10.4 MB (10446098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a85edeaa46fe5e0185f11a1a1801c0d0458e59897d3c04e97136df1c496663`  
		Last Modified: Thu, 24 Jun 2021 18:40:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:31130c0111ca19a1dca906ee7b2cc380f8e67ab892979cf56bb190c094f1522f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13173628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd0ea8d539e938e13773b20a1ea1796adb72671700cb9b65b480a669b6e3f8d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 16:38:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sun, 27 Jun 2021 16:38:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sun, 27 Jun 2021 16:38:15 GMT
ENV CADDY_VERSION=v2.4.3
# Sun, 27 Jun 2021 16:38:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sun, 27 Jun 2021 16:38:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sun, 27 Jun 2021 16:38:32 GMT
ENV XDG_CONFIG_HOME=/config
# Sun, 27 Jun 2021 16:38:34 GMT
ENV XDG_DATA_HOME=/data
# Sun, 27 Jun 2021 16:38:36 GMT
VOLUME [/config]
# Sun, 27 Jun 2021 16:38:40 GMT
VOLUME [/data]
# Sun, 27 Jun 2021 16:38:42 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sun, 27 Jun 2021 16:38:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Sun, 27 Jun 2021 16:38:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sun, 27 Jun 2021 16:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sun, 27 Jun 2021 16:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sun, 27 Jun 2021 16:38:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sun, 27 Jun 2021 16:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sun, 27 Jun 2021 16:38:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sun, 27 Jun 2021 16:39:01 GMT
EXPOSE 80
# Sun, 27 Jun 2021 16:39:03 GMT
EXPOSE 443
# Sun, 27 Jun 2021 16:39:07 GMT
EXPOSE 2019
# Sun, 27 Jun 2021 16:39:10 GMT
WORKDIR /srv
# Sun, 27 Jun 2021 16:39:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd997e1dce51da7846f8347657708b8750a0eb8c5e786c5fcef5547e42d3e9c`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 302.5 KB (302543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65a4be1a04251210dcf5d4925c25d6f9079b4bf699f80e43a2513e46421a5`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 5.9 KB (5851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f2bf16517247de92fb2f9a568c2775d92d15e09db858d1f639199eb8da303`  
		Last Modified: Sun, 27 Jun 2021 16:40:25 GMT  
		Size: 10.1 MB (10051940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca33938766a68ae61be1de59d35bcd5b4bcc18ae96c77ab8baee9b7e319e6b22`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:d4226a6c30e268159cbeb15e993d2320d162574b7dae654c2271619b3549bc04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14005935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f8604d50d95bbca3ab5038252554f7698f3fd2db7fbfeea946eae909416ae3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 04:05:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 26 Jun 2021 04:05:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 26 Jun 2021 04:05:30 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 26 Jun 2021 04:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_DATA_HOME=/data
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/config]
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/data]
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 26 Jun 2021 04:05:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 80
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 443
# Sat, 26 Jun 2021 04:05:42 GMT
EXPOSE 2019
# Sat, 26 Jun 2021 04:05:43 GMT
WORKDIR /srv
# Sat, 26 Jun 2021 04:05:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ffceb760cf41b73b97483b655680373ee04134e25bd41117589abadd6e8a82`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 300.8 KB (300839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e000d9bc18af630be9c570949ab0cddf3abec807b8ece78ce1d04846f41d296`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6100af0b373c529e22557cf3884882d8e6893ed368d5db1cbd63bf8529c98f6`  
		Last Modified: Sat, 26 Jun 2021 04:06:37 GMT  
		Size: 11.1 MB (11096440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce8db7df9776b5a33fa86bfa4ee4aa4f5167c8c0f5fd89be151b169616edd8`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:0f792d7cd96708d297fd55304917c1cad5e71b9317e68f167204d9d9e0f44657
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
$ docker pull caddy@sha256:77f27025e0e1e0ab97bc931db61d24f9ac41591e17576ab46c4b508afbccacd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14648199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8a741f4852592d8634aa37c7f351ae4f4e7b4a9a2594df54603ac48cbdad74`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 19:19:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 19:19:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 19:19:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 19:19:32 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 19:19:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 443
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 19:19:34 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 19:19:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d589bc046eca71df600301462981053bf178fcd31d4b2c882ca05aec70bacd`  
		Last Modified: Thu, 24 Jun 2021 19:19:59 GMT  
		Size: 11.5 MB (11529821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8ce9421f330c9a085ac8f059d2dd53feabf795c461d4f43b596d0302b1cf9`  
		Last Modified: Thu, 24 Jun 2021 19:19:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:276a06d4fac1a2986e5cade46d37a49e0954fb38a3b5ba846293c68ceef54d58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13816591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e555ad7d2e3449d758dae401706b4cc380e9747165f31c57760faa52fb6174a3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 18:50:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 24 Jun 2021 18:50:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:50:24 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:50:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:50:30 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:50:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:50:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:50:34 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:50:36 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:50:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e861f8792ad39fcefd1d13a12171eb53b6c830fc9182b96acb8bfb97c770fe4`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 300.5 KB (300519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd197178893bbfb4025a2b9c5edf60d3cd30075037c42b24c7b2b31bb8e559`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a2958808e8ef8313c312955baf1311cd2c15671f9d1ca3f59b720bd3c03ad`  
		Last Modified: Thu, 24 Jun 2021 18:52:04 GMT  
		Size: 10.9 MB (10887935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902e2228deaccfd2eec0d2ed45f03d38e9a341e018d1bacff231874d0b8b051`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:975e2acc21fa69679cd59786b1ecd7cf3d8f4ac40b028d61c219fd4e770d14cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88d5f2ec732bdfe5c5785fb90e7258f29e158c1857de067fb62436a723ec081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 04:25:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Jun 2021 04:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Fri, 25 Jun 2021 04:25:57 GMT
ENV CADDY_VERSION=v2.4.3
# Fri, 25 Jun 2021 04:26:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Jun 2021 04:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/config]
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/data]
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Jun 2021 04:26:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 80
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 443
# Fri, 25 Jun 2021 04:26:09 GMT
EXPOSE 2019
# Fri, 25 Jun 2021 04:26:09 GMT
WORKDIR /srv
# Fri, 25 Jun 2021 04:26:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532875903768e2aaa022f0dcc8d36d882e8a7af7edf14e86e6444c2406af868e`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 299.7 KB (299661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141d604c45916aa77667e44622bc085ab97eec4f8ba487d6f06aed74e53395a4`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e46c35d91cdc127af615f56a9074bd03baf63f40550c10ac1e56edf111fd4e`  
		Last Modified: Fri, 25 Jun 2021 04:27:42 GMT  
		Size: 10.9 MB (10863654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7106f92e86cc0f43d86170e3424675fb1543f58df755ce212946b44d5c96c38`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:780ee1b9ce06277bd5c34b2d9a6908cdb3028aa838fa75e5c6e1e32d2cabb417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13464756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a697a3b5305c041fd956ba80c8845676041e98bce128a69e70074e5abe9653dd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:39:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:39:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:39:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:39:33 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:39:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75403ccf5c23126b5dca334871ec0096a90d0fb85f47be1ecba3904921529c0`  
		Last Modified: Thu, 24 Jun 2021 18:40:18 GMT  
		Size: 10.4 MB (10446098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a85edeaa46fe5e0185f11a1a1801c0d0458e59897d3c04e97136df1c496663`  
		Last Modified: Thu, 24 Jun 2021 18:40:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:31130c0111ca19a1dca906ee7b2cc380f8e67ab892979cf56bb190c094f1522f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13173628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd0ea8d539e938e13773b20a1ea1796adb72671700cb9b65b480a669b6e3f8d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 16:38:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sun, 27 Jun 2021 16:38:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sun, 27 Jun 2021 16:38:15 GMT
ENV CADDY_VERSION=v2.4.3
# Sun, 27 Jun 2021 16:38:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sun, 27 Jun 2021 16:38:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sun, 27 Jun 2021 16:38:32 GMT
ENV XDG_CONFIG_HOME=/config
# Sun, 27 Jun 2021 16:38:34 GMT
ENV XDG_DATA_HOME=/data
# Sun, 27 Jun 2021 16:38:36 GMT
VOLUME [/config]
# Sun, 27 Jun 2021 16:38:40 GMT
VOLUME [/data]
# Sun, 27 Jun 2021 16:38:42 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sun, 27 Jun 2021 16:38:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Sun, 27 Jun 2021 16:38:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sun, 27 Jun 2021 16:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sun, 27 Jun 2021 16:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sun, 27 Jun 2021 16:38:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sun, 27 Jun 2021 16:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sun, 27 Jun 2021 16:38:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sun, 27 Jun 2021 16:39:01 GMT
EXPOSE 80
# Sun, 27 Jun 2021 16:39:03 GMT
EXPOSE 443
# Sun, 27 Jun 2021 16:39:07 GMT
EXPOSE 2019
# Sun, 27 Jun 2021 16:39:10 GMT
WORKDIR /srv
# Sun, 27 Jun 2021 16:39:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd997e1dce51da7846f8347657708b8750a0eb8c5e786c5fcef5547e42d3e9c`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 302.5 KB (302543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65a4be1a04251210dcf5d4925c25d6f9079b4bf699f80e43a2513e46421a5`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 5.9 KB (5851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f2bf16517247de92fb2f9a568c2775d92d15e09db858d1f639199eb8da303`  
		Last Modified: Sun, 27 Jun 2021 16:40:25 GMT  
		Size: 10.1 MB (10051940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca33938766a68ae61be1de59d35bcd5b4bcc18ae96c77ab8baee9b7e319e6b22`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d4226a6c30e268159cbeb15e993d2320d162574b7dae654c2271619b3549bc04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14005935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f8604d50d95bbca3ab5038252554f7698f3fd2db7fbfeea946eae909416ae3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 04:05:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 26 Jun 2021 04:05:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 26 Jun 2021 04:05:30 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 26 Jun 2021 04:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_DATA_HOME=/data
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/config]
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/data]
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 26 Jun 2021 04:05:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 80
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 443
# Sat, 26 Jun 2021 04:05:42 GMT
EXPOSE 2019
# Sat, 26 Jun 2021 04:05:43 GMT
WORKDIR /srv
# Sat, 26 Jun 2021 04:05:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ffceb760cf41b73b97483b655680373ee04134e25bd41117589abadd6e8a82`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 300.8 KB (300839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e000d9bc18af630be9c570949ab0cddf3abec807b8ece78ce1d04846f41d296`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6100af0b373c529e22557cf3884882d8e6893ed368d5db1cbd63bf8529c98f6`  
		Last Modified: Sat, 26 Jun 2021 04:06:37 GMT  
		Size: 11.1 MB (11096440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce8db7df9776b5a33fa86bfa4ee4aa4f5167c8c0f5fd89be151b169616edd8`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:a67ad5e8b31cce8d525433db1ed70bcf31dadb0a6232fede113d6aa29ff6bd9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:f6cdd65e955bc74496559b799a16c919549831ca75ccfc32dc5ef04d1fc4e5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116854935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871368d0c2131d992e382b9e0d4ade9b0ff877237c1f08e1f0439744ae010b4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:20:03 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:20:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:20:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:29 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:44:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 00:44:31 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:44:32 GMT
WORKDIR /go
# Tue, 13 Jul 2021 22:43:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 22:43:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 22:43:41 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 22:43:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 22:43:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 22:43:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 22:43:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8dd7cab73593e079aa6f5b2fe6c2adfe09761320c162696f8fbdc9d81c99e6`  
		Last Modified: Fri, 25 Jun 2021 23:16:30 GMT  
		Size: 281.5 KB (281504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac70760d29a8ed86a3f007ed2410ef62cc877ddd2ceaa3e10806664fb3d1d1`  
		Last Modified: Fri, 25 Jun 2021 23:16:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edffed539bd83dee46e0e9cad74f38623ec3cd1cdafa538a8f390f1ce3dad86`  
		Last Modified: Tue, 13 Jul 2021 00:57:36 GMT  
		Size: 105.8 MB (105823516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4005d2dc874b23b426670e96f7fd6fb135e699c7424968915b39092a6c65413`  
		Last Modified: Tue, 13 Jul 2021 00:57:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707db5879f70d57e47f626fefe4da13194e93987052fbb6abafadb7ffdd1baf`  
		Last Modified: Tue, 13 Jul 2021 22:44:16 GMT  
		Size: 6.6 MB (6626557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692866fb377b59f86eaf10234066d2f1d916074aa34c13847cbb0caf5e69bbcd`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 1.3 MB (1311164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b20931cdefb4b7578f01983d447a9eca419f53d6587b66df256aed35a14da`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3787ea93f75ebc3f9acdcbec6135c116e5efa2a9c636444bd0c6d0ad31a3c9c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112615087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4069a24bc8333ba2b78088aca22dd8150c4f7187e4f841170e050c5c1eac3f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 22:27:47 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 25 Jun 2021 22:27:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 22:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:55:15 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:57:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:57:52 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:57:55 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:11:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:11:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:11:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:11:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:11:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:11:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:11:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59daecef61f9012ed738a38ec0c69536f19c402ec68bf2b4e41224f4691ea6`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 281.7 KB (281675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33922e4ea9c90b51975f02a97ef9af96446749dc32fec4bce4f81472d5951f4c`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db3f5706e49257fa734663b30ecab76ade215386fee8d45fbe528732c8ad236`  
		Last Modified: Tue, 13 Jul 2021 02:13:03 GMT  
		Size: 102.0 MB (102002367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cfd82c985c779e28d38d13ffdd4ce57037f731afaafa87e18fa7765ccfecfa`  
		Last Modified: Tue, 13 Jul 2021 02:11:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c454daa6f4a8717d038ea20ff8db8fb988026d0e76d710c3d33ede81f6cf`  
		Last Modified: Tue, 13 Jul 2021 03:12:33 GMT  
		Size: 6.5 MB (6484276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b99595e2bdb02f0ad02d7a5bcdedce9128a3dda75833df312c3c810d8db36`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 1.2 MB (1221671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420863b180db807f8dc3c690d70856904ed5564edad8b7c4fdcce313b5637ac8`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aff38fe0c8e1a1865b4d77f303f470dda0b940df6cd371d6902c2a65807ed46e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111530985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eaed7b8bc79805b49774a853bb94da8830a86f9891a687fb782da38eb75c9e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 17:37:55 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 24 Jun 2021 17:37:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 17:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:43 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:07:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 06:07:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:07:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:07:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:07:21 GMT
WORKDIR /go
# Tue, 13 Jul 2021 10:23:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 10:23:22 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 10:23:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 10:23:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 10:23:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 10:23:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 10:23:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b6a653704b1a4485c078013594b13c6802997d9ee3aaadab95a9f5537d90fb`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 280.8 KB (280816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d159d413b624554c6f7f204b6631e5e0ffa0d8dcaecc7c187ee02b1a3046c8d`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62dae21018e5e16e900f01a5fb7663f2b12428b921c4aa202eaa3a8d0ac325`  
		Last Modified: Tue, 13 Jul 2021 06:31:05 GMT  
		Size: 101.8 MB (101818292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d2950946468eaf7199de14481fbdaf85b1d5887fba133ca2b322a552b1432`  
		Last Modified: Tue, 13 Jul 2021 06:29:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f2d2adb1c355d81282e49ce092a2bb83ee4c9d22b5bb108f7f5c285a64cdca`  
		Last Modified: Tue, 13 Jul 2021 10:24:35 GMT  
		Size: 5.8 MB (5783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9049b6efaa99533b580d82c04dfc8ef9a5427d766dd1318dc3a197cc1c1c963c`  
		Last Modified: Tue, 13 Jul 2021 10:24:34 GMT  
		Size: 1.2 MB (1219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50232af76c17b758457793588aadd38c6893d1e444164ff0cc52a2c21175ecb5`  
		Last Modified: Tue, 13 Jul 2021 10:24:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:34954aa0c8992528f20e69e7ab2924ba4a6422c90a8368468fec8644ba863c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112071299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e9b3de118d54351f56b411cfdb409214e141f9a7f07456c84c7591a164079`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:52:32 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:52:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:51 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:43:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:43:14 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:43:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:43:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:43:16 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:42:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:42:15 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:42:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:42:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:42:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:42:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ad96702509b3443881ad70a623b6184f9936c6b4cd986694020c95f3a4441c`  
		Last Modified: Fri, 25 Jun 2021 22:11:26 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bf5f5ed4dc23e2dc33456ba3ccbef3ecabf22614e760a8f4c1e3a93a6c59b`  
		Last Modified: Fri, 25 Jun 2021 22:11:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec328162280f19fa491a9223100438095ce2a77e7b9281df21e7be3bd6a7bc4`  
		Last Modified: Tue, 13 Jul 2021 01:54:27 GMT  
		Size: 101.1 MB (101142101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19e5d43a5efe6c746a1cfa2fcf1862bcc4925567d86a5c59e84ff2e1e1e9ff`  
		Last Modified: Tue, 13 Jul 2021 01:54:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527df0ff5cb43607ace2d4f041155956865d5a96f792dde6e0bc61d933aa00`  
		Last Modified: Tue, 13 Jul 2021 03:42:55 GMT  
		Size: 6.7 MB (6735645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8330a61ff9dad4df609f84bed371e68bfc277e4f5d732ef213a7a91eb2a10c4`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fcafea7f32c7cecd033dfdc40ee8ef68a394474a4db2622e529fbf14f25bd`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:74dd51e67bac5134b07d790c2346426390de3753497b1eec9bab0824e2a77232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110953352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a48de21654c9b62f43aa4fe92a4247925e90604819de1650fdcb71d8ee8b79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Tue, 20 Jul 2021 18:17:13 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Jul 2021 18:17:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Jul 2021 18:18:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jul 2021 18:21:22 GMT
ENV GOLANG_VERSION=1.16.6
# Fri, 23 Jul 2021 04:40:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 23 Jul 2021 04:40:28 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 04:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 04:41:02 GMT
WORKDIR /go
# Sat, 24 Jul 2021 05:19:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 24 Jul 2021 05:20:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 24 Jul 2021 05:20:02 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 24 Jul 2021 05:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 24 Jul 2021 05:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 24 Jul 2021 05:20:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 24 Jul 2021 05:20:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721ce277ce9262c870e1d352522e195d85ab25af4583839398f9a01c38b3dc2e`  
		Last Modified: Fri, 23 Jul 2021 04:48:01 GMT  
		Size: 283.6 KB (283650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ebf56dbf1e11bd67d55495e34cb5c84af755e9dfcaf65988531ce52a39e5d2`  
		Last Modified: Fri, 23 Jul 2021 04:48:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8592af8ad492e633c5ab1d6aa7fff04c4cfff50cbb68ad82b016ec2a1e62bb`  
		Last Modified: Fri, 23 Jul 2021 04:49:38 GMT  
		Size: 99.6 MB (99590623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600ce69bae4413214508296d621077daf64be996fb54771a68137369cc8134b`  
		Last Modified: Fri, 23 Jul 2021 04:49:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8187500a8da9f9367453b30682a867757b6194435eea42ed2f0a45d9fc7e3bfe`  
		Last Modified: Sat, 24 Jul 2021 05:20:51 GMT  
		Size: 7.1 MB (7097373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3c9911a962be6147627de3fe9b3fd513faa943eb1ab047dd5985756ff251f`  
		Last Modified: Sat, 24 Jul 2021 05:20:50 GMT  
		Size: 1.2 MB (1170514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ad770096fea4fb91c8cd35ad172b5de002fa541d7f2fb806ce9333949d561`  
		Last Modified: Sat, 24 Jul 2021 05:20:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c1fe90d100bc65dda91fdf5bdb63f816e99fc4a9928e147d2751b3a7d9d18cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc2a6a4ddf246e8517f51a95c8d6b19ea5ce09cfe97c2dc1a044bd2df444116`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Sat, 26 Jun 2021 04:05:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 26 Jun 2021 04:05:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 26 Jun 2021 04:05:55 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Jun 2021 04:05:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 26 Jun 2021 04:05:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 26 Jun 2021 04:05:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eee054ded34b1fa082776278b24e58f3711d292231b9317ab8e3596dcade07c`  
		Last Modified: Sat, 26 Jun 2021 04:06:48 GMT  
		Size: 6.5 MB (6479052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a8988e62b4b7bdcd1f3d58ab8e59e5fa2ab7ed6eca36ccfaf85f5d18eb4f5`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 1.3 MB (1264519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038b88769d2da3d3539b44720ea6f58fe16e59cf4a2e6a92ac601da04c7a51d`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:4eb06e332fdb2d502f24125aa931d24cde59802a343c6488069fb94a54ef74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852362865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e315378f9d8c30da3455c154df8d7f7363d22371e702839e334120dca02f0d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:25:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:25:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:25:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:25:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:27:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:27:07 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:28:09 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:42:39 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:45:55 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:45:59 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 17:59:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:59:42 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 17:59:45 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:59:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:00:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:01:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c50202491861e9cc59ef0cad62ab13b4d8585699abaf13275f815b0ab53bf`  
		Last Modified: Wed, 14 Jul 2021 05:03:35 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700aac46fe704c190ed71a3f8ec8f1eca6d0fed9861862fcab96996d21678657`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce5c766a8b7a15e6b68bef29d1932c4e9cf7086c6413acfcb35b89e6363813f`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3527d984880519c45793ad5f901d15605068f0a52a819044cd79ded461f09`  
		Last Modified: Wed, 14 Jul 2021 05:03:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f16e3c9a35398857e96f60776b71b2af7e30419946307d58f942fe090b2f9`  
		Last Modified: Wed, 14 Jul 2021 05:04:02 GMT  
		Size: 25.5 MB (25460385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0876037206b7bfb610c4f7906510321d8255635221cabe7945218bd0e4d6675`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e278916db542be6afd74117c73ed9743e7cdb1de94d1928e2ba00faeff6334e`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 334.2 KB (334178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b10c3fa755eb4b8899c649883154bdfabb4d8210fd05c99501bd914ac9b731`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1c58792690c81eb4a6642c459efd28697c5ff8929b42470cee6a7e4082ee1`  
		Last Modified: Wed, 14 Jul 2021 05:06:35 GMT  
		Size: 139.4 MB (139379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1825c045e930c77550f32b2d4b24f4fa8753d0cf7020f4c51ea28af9d52b89e`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.6 KB (1575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc30c19fc7720ff29534e571e8e5a1673c2675f67c177298f208911bcbc1f96`  
		Last Modified: Wed, 14 Jul 2021 18:04:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9e2c7d361d98c4325e76790bce3765156415850f328aaae18799eca52ba3a`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6d93b9213829269ca2cb4b45b481f1143b1aecbd8def9e9cd79d2d19a666`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5897ea6c031bde10f5b5ddabe05c5f99d99f378bd12f47b9c0962b4416e20cd6`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31be288471040830a89925530422731817f7d69131073c3b77722fcf1001414`  
		Last Modified: Wed, 14 Jul 2021 18:04:52 GMT  
		Size: 1.7 MB (1723702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e061480b37961b0add8ffa998c3d22f956b4722aa569338bc029a923d3ac6`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:64455ff9cc52a6eaa711eafb2f11ebc5fa78a5f15e7c1be1e4a05d2039c5eb04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6440905132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46bc0ac245d8871ca7a2ef877724591c00e6f40eb64608a40f20e5728bdd7ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:31:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:31:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:31:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:33:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:33:36 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:35:06 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:46:08 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:49:49 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:49:53 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 18:01:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:01:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 18:01:27 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 18:01:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:03:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:03:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f667c0fc8186714bfddbd565e9cdd1dd6497e3c112f1eddb17a37d1abae30c93`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3566f190f34782035012abf2530315039000f1d137ad0098f1903a99127b3b8e`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036fdd63bb05506922a2462b2487bb4ff12b9c29097537ee7d0ca4c18cad7507`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904dd19478585c0fa1c9b4a25c5ac4560759b61f3f9e2ef0e6475729d5d482`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a50006063e099df0e3d1f22baa504b0f0de1563cd642c48340cf2a8b7152bd`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 25.4 MB (25447622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445d6d1bd7224c109fda54abaaa5909b43be941934bc54c3aff8754b852ebd`  
		Last Modified: Wed, 14 Jul 2021 05:04:20 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0187f6db85279d8f0ab2b263b47845afa4452a66c28c251f571d776001e4d300`  
		Last Modified: Wed, 14 Jul 2021 05:04:21 GMT  
		Size: 318.8 KB (318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a18e3af73fb6a22be9e13447c4dc03d831112dcc5d479c52c994c324b1bca`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b18fe05fb046103c962da798acc46523e448a87265015bd0e9870d49013e2`  
		Last Modified: Wed, 14 Jul 2021 05:07:32 GMT  
		Size: 143.8 MB (143795404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eacae5fc4eee1b8807585646451e54ef2f58b632b6d045038d647606936b8f`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9145f72acba1daf6003e68907818ef42985c05eb03e5eb0886fd4f833a7b916d`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c947cad69b975374c14de848aaa54c4a57260a151a320dbe96a6348db9a8a200`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f30145eea91938fd9fabc5f8f26fe49414b7c7807a32d8cba919c9e493f826f`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eadb657f23ec662680db8a9bc4e1ade309bf93d0203e4b1c07fccf629772aa`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0920c1f5b52107603b2811da4a1f8d4d3582979217761675db22876a07e3cd`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.7 MB (1693422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239173a5587fc73012d57cf4f1387c28f9bb618c4bb423eaa0656dce5585a5c`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:5127c38c6131f5d14b322516c0b88e8b1a6b41acc126856a7f28a677d06b5f07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:f6cdd65e955bc74496559b799a16c919549831ca75ccfc32dc5ef04d1fc4e5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116854935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871368d0c2131d992e382b9e0d4ade9b0ff877237c1f08e1f0439744ae010b4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:20:03 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:20:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:20:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:29 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:44:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 00:44:31 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:44:32 GMT
WORKDIR /go
# Tue, 13 Jul 2021 22:43:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 22:43:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 22:43:41 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 22:43:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 22:43:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 22:43:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 22:43:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8dd7cab73593e079aa6f5b2fe6c2adfe09761320c162696f8fbdc9d81c99e6`  
		Last Modified: Fri, 25 Jun 2021 23:16:30 GMT  
		Size: 281.5 KB (281504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac70760d29a8ed86a3f007ed2410ef62cc877ddd2ceaa3e10806664fb3d1d1`  
		Last Modified: Fri, 25 Jun 2021 23:16:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edffed539bd83dee46e0e9cad74f38623ec3cd1cdafa538a8f390f1ce3dad86`  
		Last Modified: Tue, 13 Jul 2021 00:57:36 GMT  
		Size: 105.8 MB (105823516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4005d2dc874b23b426670e96f7fd6fb135e699c7424968915b39092a6c65413`  
		Last Modified: Tue, 13 Jul 2021 00:57:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707db5879f70d57e47f626fefe4da13194e93987052fbb6abafadb7ffdd1baf`  
		Last Modified: Tue, 13 Jul 2021 22:44:16 GMT  
		Size: 6.6 MB (6626557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692866fb377b59f86eaf10234066d2f1d916074aa34c13847cbb0caf5e69bbcd`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 1.3 MB (1311164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b20931cdefb4b7578f01983d447a9eca419f53d6587b66df256aed35a14da`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3787ea93f75ebc3f9acdcbec6135c116e5efa2a9c636444bd0c6d0ad31a3c9c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112615087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4069a24bc8333ba2b78088aca22dd8150c4f7187e4f841170e050c5c1eac3f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 22:27:47 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 25 Jun 2021 22:27:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 22:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:55:15 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:57:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:57:52 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:57:55 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:11:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:11:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:11:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:11:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:11:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:11:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:11:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59daecef61f9012ed738a38ec0c69536f19c402ec68bf2b4e41224f4691ea6`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 281.7 KB (281675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33922e4ea9c90b51975f02a97ef9af96446749dc32fec4bce4f81472d5951f4c`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db3f5706e49257fa734663b30ecab76ade215386fee8d45fbe528732c8ad236`  
		Last Modified: Tue, 13 Jul 2021 02:13:03 GMT  
		Size: 102.0 MB (102002367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cfd82c985c779e28d38d13ffdd4ce57037f731afaafa87e18fa7765ccfecfa`  
		Last Modified: Tue, 13 Jul 2021 02:11:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c454daa6f4a8717d038ea20ff8db8fb988026d0e76d710c3d33ede81f6cf`  
		Last Modified: Tue, 13 Jul 2021 03:12:33 GMT  
		Size: 6.5 MB (6484276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b99595e2bdb02f0ad02d7a5bcdedce9128a3dda75833df312c3c810d8db36`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 1.2 MB (1221671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420863b180db807f8dc3c690d70856904ed5564edad8b7c4fdcce313b5637ac8`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aff38fe0c8e1a1865b4d77f303f470dda0b940df6cd371d6902c2a65807ed46e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111530985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eaed7b8bc79805b49774a853bb94da8830a86f9891a687fb782da38eb75c9e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 17:37:55 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 24 Jun 2021 17:37:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 17:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:43 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:07:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 06:07:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:07:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:07:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:07:21 GMT
WORKDIR /go
# Tue, 13 Jul 2021 10:23:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 10:23:22 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 10:23:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 10:23:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 10:23:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 10:23:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 10:23:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b6a653704b1a4485c078013594b13c6802997d9ee3aaadab95a9f5537d90fb`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 280.8 KB (280816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d159d413b624554c6f7f204b6631e5e0ffa0d8dcaecc7c187ee02b1a3046c8d`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62dae21018e5e16e900f01a5fb7663f2b12428b921c4aa202eaa3a8d0ac325`  
		Last Modified: Tue, 13 Jul 2021 06:31:05 GMT  
		Size: 101.8 MB (101818292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d2950946468eaf7199de14481fbdaf85b1d5887fba133ca2b322a552b1432`  
		Last Modified: Tue, 13 Jul 2021 06:29:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f2d2adb1c355d81282e49ce092a2bb83ee4c9d22b5bb108f7f5c285a64cdca`  
		Last Modified: Tue, 13 Jul 2021 10:24:35 GMT  
		Size: 5.8 MB (5783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9049b6efaa99533b580d82c04dfc8ef9a5427d766dd1318dc3a197cc1c1c963c`  
		Last Modified: Tue, 13 Jul 2021 10:24:34 GMT  
		Size: 1.2 MB (1219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50232af76c17b758457793588aadd38c6893d1e444164ff0cc52a2c21175ecb5`  
		Last Modified: Tue, 13 Jul 2021 10:24:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:34954aa0c8992528f20e69e7ab2924ba4a6422c90a8368468fec8644ba863c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112071299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e9b3de118d54351f56b411cfdb409214e141f9a7f07456c84c7591a164079`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:52:32 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:52:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:51 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:43:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:43:14 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:43:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:43:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:43:16 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:42:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:42:15 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:42:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:42:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:42:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:42:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ad96702509b3443881ad70a623b6184f9936c6b4cd986694020c95f3a4441c`  
		Last Modified: Fri, 25 Jun 2021 22:11:26 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bf5f5ed4dc23e2dc33456ba3ccbef3ecabf22614e760a8f4c1e3a93a6c59b`  
		Last Modified: Fri, 25 Jun 2021 22:11:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec328162280f19fa491a9223100438095ce2a77e7b9281df21e7be3bd6a7bc4`  
		Last Modified: Tue, 13 Jul 2021 01:54:27 GMT  
		Size: 101.1 MB (101142101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19e5d43a5efe6c746a1cfa2fcf1862bcc4925567d86a5c59e84ff2e1e1e9ff`  
		Last Modified: Tue, 13 Jul 2021 01:54:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527df0ff5cb43607ace2d4f041155956865d5a96f792dde6e0bc61d933aa00`  
		Last Modified: Tue, 13 Jul 2021 03:42:55 GMT  
		Size: 6.7 MB (6735645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8330a61ff9dad4df609f84bed371e68bfc277e4f5d732ef213a7a91eb2a10c4`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fcafea7f32c7cecd033dfdc40ee8ef68a394474a4db2622e529fbf14f25bd`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:74dd51e67bac5134b07d790c2346426390de3753497b1eec9bab0824e2a77232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110953352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a48de21654c9b62f43aa4fe92a4247925e90604819de1650fdcb71d8ee8b79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Tue, 20 Jul 2021 18:17:13 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Jul 2021 18:17:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Jul 2021 18:18:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jul 2021 18:21:22 GMT
ENV GOLANG_VERSION=1.16.6
# Fri, 23 Jul 2021 04:40:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 23 Jul 2021 04:40:28 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 04:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 04:41:02 GMT
WORKDIR /go
# Sat, 24 Jul 2021 05:19:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 24 Jul 2021 05:20:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 24 Jul 2021 05:20:02 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 24 Jul 2021 05:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 24 Jul 2021 05:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 24 Jul 2021 05:20:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 24 Jul 2021 05:20:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721ce277ce9262c870e1d352522e195d85ab25af4583839398f9a01c38b3dc2e`  
		Last Modified: Fri, 23 Jul 2021 04:48:01 GMT  
		Size: 283.6 KB (283650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ebf56dbf1e11bd67d55495e34cb5c84af755e9dfcaf65988531ce52a39e5d2`  
		Last Modified: Fri, 23 Jul 2021 04:48:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8592af8ad492e633c5ab1d6aa7fff04c4cfff50cbb68ad82b016ec2a1e62bb`  
		Last Modified: Fri, 23 Jul 2021 04:49:38 GMT  
		Size: 99.6 MB (99590623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600ce69bae4413214508296d621077daf64be996fb54771a68137369cc8134b`  
		Last Modified: Fri, 23 Jul 2021 04:49:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8187500a8da9f9367453b30682a867757b6194435eea42ed2f0a45d9fc7e3bfe`  
		Last Modified: Sat, 24 Jul 2021 05:20:51 GMT  
		Size: 7.1 MB (7097373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3c9911a962be6147627de3fe9b3fd513faa943eb1ab047dd5985756ff251f`  
		Last Modified: Sat, 24 Jul 2021 05:20:50 GMT  
		Size: 1.2 MB (1170514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ad770096fea4fb91c8cd35ad172b5de002fa541d7f2fb806ce9333949d561`  
		Last Modified: Sat, 24 Jul 2021 05:20:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1c1fe90d100bc65dda91fdf5bdb63f816e99fc4a9928e147d2751b3a7d9d18cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc2a6a4ddf246e8517f51a95c8d6b19ea5ce09cfe97c2dc1a044bd2df444116`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Sat, 26 Jun 2021 04:05:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 26 Jun 2021 04:05:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 26 Jun 2021 04:05:55 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Jun 2021 04:05:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 26 Jun 2021 04:05:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 26 Jun 2021 04:05:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eee054ded34b1fa082776278b24e58f3711d292231b9317ab8e3596dcade07c`  
		Last Modified: Sat, 26 Jun 2021 04:06:48 GMT  
		Size: 6.5 MB (6479052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a8988e62b4b7bdcd1f3d58ab8e59e5fa2ab7ed6eca36ccfaf85f5d18eb4f5`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 1.3 MB (1264519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038b88769d2da3d3539b44720ea6f58fe16e59cf4a2e6a92ac601da04c7a51d`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:19c88ab0becc5cc1a1361c8307d1a87c8f2b9f28eff7f34a7abe19090c6cdef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:4eb06e332fdb2d502f24125aa931d24cde59802a343c6488069fb94a54ef74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852362865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e315378f9d8c30da3455c154df8d7f7363d22371e702839e334120dca02f0d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:25:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:25:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:25:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:25:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:27:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:27:07 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:28:09 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:42:39 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:45:55 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:45:59 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 17:59:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:59:42 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 17:59:45 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:59:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:00:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:01:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c50202491861e9cc59ef0cad62ab13b4d8585699abaf13275f815b0ab53bf`  
		Last Modified: Wed, 14 Jul 2021 05:03:35 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700aac46fe704c190ed71a3f8ec8f1eca6d0fed9861862fcab96996d21678657`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce5c766a8b7a15e6b68bef29d1932c4e9cf7086c6413acfcb35b89e6363813f`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3527d984880519c45793ad5f901d15605068f0a52a819044cd79ded461f09`  
		Last Modified: Wed, 14 Jul 2021 05:03:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f16e3c9a35398857e96f60776b71b2af7e30419946307d58f942fe090b2f9`  
		Last Modified: Wed, 14 Jul 2021 05:04:02 GMT  
		Size: 25.5 MB (25460385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0876037206b7bfb610c4f7906510321d8255635221cabe7945218bd0e4d6675`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e278916db542be6afd74117c73ed9743e7cdb1de94d1928e2ba00faeff6334e`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 334.2 KB (334178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b10c3fa755eb4b8899c649883154bdfabb4d8210fd05c99501bd914ac9b731`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1c58792690c81eb4a6642c459efd28697c5ff8929b42470cee6a7e4082ee1`  
		Last Modified: Wed, 14 Jul 2021 05:06:35 GMT  
		Size: 139.4 MB (139379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1825c045e930c77550f32b2d4b24f4fa8753d0cf7020f4c51ea28af9d52b89e`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.6 KB (1575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc30c19fc7720ff29534e571e8e5a1673c2675f67c177298f208911bcbc1f96`  
		Last Modified: Wed, 14 Jul 2021 18:04:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9e2c7d361d98c4325e76790bce3765156415850f328aaae18799eca52ba3a`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6d93b9213829269ca2cb4b45b481f1143b1aecbd8def9e9cd79d2d19a666`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5897ea6c031bde10f5b5ddabe05c5f99d99f378bd12f47b9c0962b4416e20cd6`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31be288471040830a89925530422731817f7d69131073c3b77722fcf1001414`  
		Last Modified: Wed, 14 Jul 2021 18:04:52 GMT  
		Size: 1.7 MB (1723702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e061480b37961b0add8ffa998c3d22f956b4722aa569338bc029a923d3ac6`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f0154eaa9e2dbf0c3cdcaff8538332c786fe497522a1e2277d7bee2afa8829e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:64455ff9cc52a6eaa711eafb2f11ebc5fa78a5f15e7c1be1e4a05d2039c5eb04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6440905132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46bc0ac245d8871ca7a2ef877724591c00e6f40eb64608a40f20e5728bdd7ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:31:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:31:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:31:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:33:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:33:36 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:35:06 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:46:08 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:49:49 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:49:53 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 18:01:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:01:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 18:01:27 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 18:01:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:03:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:03:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f667c0fc8186714bfddbd565e9cdd1dd6497e3c112f1eddb17a37d1abae30c93`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3566f190f34782035012abf2530315039000f1d137ad0098f1903a99127b3b8e`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036fdd63bb05506922a2462b2487bb4ff12b9c29097537ee7d0ca4c18cad7507`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904dd19478585c0fa1c9b4a25c5ac4560759b61f3f9e2ef0e6475729d5d482`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a50006063e099df0e3d1f22baa504b0f0de1563cd642c48340cf2a8b7152bd`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 25.4 MB (25447622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445d6d1bd7224c109fda54abaaa5909b43be941934bc54c3aff8754b852ebd`  
		Last Modified: Wed, 14 Jul 2021 05:04:20 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0187f6db85279d8f0ab2b263b47845afa4452a66c28c251f571d776001e4d300`  
		Last Modified: Wed, 14 Jul 2021 05:04:21 GMT  
		Size: 318.8 KB (318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a18e3af73fb6a22be9e13447c4dc03d831112dcc5d479c52c994c324b1bca`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b18fe05fb046103c962da798acc46523e448a87265015bd0e9870d49013e2`  
		Last Modified: Wed, 14 Jul 2021 05:07:32 GMT  
		Size: 143.8 MB (143795404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eacae5fc4eee1b8807585646451e54ef2f58b632b6d045038d647606936b8f`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9145f72acba1daf6003e68907818ef42985c05eb03e5eb0886fd4f833a7b916d`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c947cad69b975374c14de848aaa54c4a57260a151a320dbe96a6348db9a8a200`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f30145eea91938fd9fabc5f8f26fe49414b7c7807a32d8cba919c9e493f826f`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eadb657f23ec662680db8a9bc4e1ade309bf93d0203e4b1c07fccf629772aa`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0920c1f5b52107603b2811da4a1f8d4d3582979217761675db22876a07e3cd`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.7 MB (1693422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239173a5587fc73012d57cf4f1387c28f9bb618c4bb423eaa0656dce5585a5c`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:7f1035763458a1b2157ab61efe3803c97713d979fe1b486a45379ccf785b0df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:3edc19bfdb3220c2ab0cdd322296d11640a5fed6927d8623bda1b75fde4db610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:ea60a37d4cd836ad64d2085c4951355657b0593ae72734ed4fae65632a0d5a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3`

```console
$ docker pull caddy@sha256:90dfeaa3846391a67e0e9dec49fbe8c3031eec18cdbb92258b2e45bcd1c775d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:2.4.3` - linux; amd64

```console
$ docker pull caddy@sha256:77f27025e0e1e0ab97bc931db61d24f9ac41591e17576ab46c4b508afbccacd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14648199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8a741f4852592d8634aa37c7f351ae4f4e7b4a9a2594df54603ac48cbdad74`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 19:19:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 19:19:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 19:19:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 19:19:32 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 19:19:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 443
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 19:19:34 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 19:19:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d589bc046eca71df600301462981053bf178fcd31d4b2c882ca05aec70bacd`  
		Last Modified: Thu, 24 Jun 2021 19:19:59 GMT  
		Size: 11.5 MB (11529821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8ce9421f330c9a085ac8f059d2dd53feabf795c461d4f43b596d0302b1cf9`  
		Last Modified: Thu, 24 Jun 2021 19:19:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3` - linux; arm variant v6

```console
$ docker pull caddy@sha256:276a06d4fac1a2986e5cade46d37a49e0954fb38a3b5ba846293c68ceef54d58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13816591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e555ad7d2e3449d758dae401706b4cc380e9747165f31c57760faa52fb6174a3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 18:50:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 24 Jun 2021 18:50:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:50:24 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:50:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:50:30 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:50:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:50:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:50:34 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:50:36 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:50:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e861f8792ad39fcefd1d13a12171eb53b6c830fc9182b96acb8bfb97c770fe4`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 300.5 KB (300519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd197178893bbfb4025a2b9c5edf60d3cd30075037c42b24c7b2b31bb8e559`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a2958808e8ef8313c312955baf1311cd2c15671f9d1ca3f59b720bd3c03ad`  
		Last Modified: Thu, 24 Jun 2021 18:52:04 GMT  
		Size: 10.9 MB (10887935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902e2228deaccfd2eec0d2ed45f03d38e9a341e018d1bacff231874d0b8b051`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3` - linux; arm variant v7

```console
$ docker pull caddy@sha256:975e2acc21fa69679cd59786b1ecd7cf3d8f4ac40b028d61c219fd4e770d14cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88d5f2ec732bdfe5c5785fb90e7258f29e158c1857de067fb62436a723ec081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 04:25:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Jun 2021 04:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Fri, 25 Jun 2021 04:25:57 GMT
ENV CADDY_VERSION=v2.4.3
# Fri, 25 Jun 2021 04:26:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Jun 2021 04:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/config]
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/data]
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Jun 2021 04:26:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 80
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 443
# Fri, 25 Jun 2021 04:26:09 GMT
EXPOSE 2019
# Fri, 25 Jun 2021 04:26:09 GMT
WORKDIR /srv
# Fri, 25 Jun 2021 04:26:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532875903768e2aaa022f0dcc8d36d882e8a7af7edf14e86e6444c2406af868e`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 299.7 KB (299661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141d604c45916aa77667e44622bc085ab97eec4f8ba487d6f06aed74e53395a4`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e46c35d91cdc127af615f56a9074bd03baf63f40550c10ac1e56edf111fd4e`  
		Last Modified: Fri, 25 Jun 2021 04:27:42 GMT  
		Size: 10.9 MB (10863654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7106f92e86cc0f43d86170e3424675fb1543f58df755ce212946b44d5c96c38`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:780ee1b9ce06277bd5c34b2d9a6908cdb3028aa838fa75e5c6e1e32d2cabb417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13464756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a697a3b5305c041fd956ba80c8845676041e98bce128a69e70074e5abe9653dd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:39:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:39:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:39:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:39:33 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:39:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75403ccf5c23126b5dca334871ec0096a90d0fb85f47be1ecba3904921529c0`  
		Last Modified: Thu, 24 Jun 2021 18:40:18 GMT  
		Size: 10.4 MB (10446098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a85edeaa46fe5e0185f11a1a1801c0d0458e59897d3c04e97136df1c496663`  
		Last Modified: Thu, 24 Jun 2021 18:40:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3` - linux; ppc64le

```console
$ docker pull caddy@sha256:31130c0111ca19a1dca906ee7b2cc380f8e67ab892979cf56bb190c094f1522f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13173628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd0ea8d539e938e13773b20a1ea1796adb72671700cb9b65b480a669b6e3f8d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 16:38:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sun, 27 Jun 2021 16:38:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sun, 27 Jun 2021 16:38:15 GMT
ENV CADDY_VERSION=v2.4.3
# Sun, 27 Jun 2021 16:38:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sun, 27 Jun 2021 16:38:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sun, 27 Jun 2021 16:38:32 GMT
ENV XDG_CONFIG_HOME=/config
# Sun, 27 Jun 2021 16:38:34 GMT
ENV XDG_DATA_HOME=/data
# Sun, 27 Jun 2021 16:38:36 GMT
VOLUME [/config]
# Sun, 27 Jun 2021 16:38:40 GMT
VOLUME [/data]
# Sun, 27 Jun 2021 16:38:42 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sun, 27 Jun 2021 16:38:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Sun, 27 Jun 2021 16:38:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sun, 27 Jun 2021 16:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sun, 27 Jun 2021 16:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sun, 27 Jun 2021 16:38:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sun, 27 Jun 2021 16:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sun, 27 Jun 2021 16:38:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sun, 27 Jun 2021 16:39:01 GMT
EXPOSE 80
# Sun, 27 Jun 2021 16:39:03 GMT
EXPOSE 443
# Sun, 27 Jun 2021 16:39:07 GMT
EXPOSE 2019
# Sun, 27 Jun 2021 16:39:10 GMT
WORKDIR /srv
# Sun, 27 Jun 2021 16:39:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd997e1dce51da7846f8347657708b8750a0eb8c5e786c5fcef5547e42d3e9c`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 302.5 KB (302543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65a4be1a04251210dcf5d4925c25d6f9079b4bf699f80e43a2513e46421a5`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 5.9 KB (5851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f2bf16517247de92fb2f9a568c2775d92d15e09db858d1f639199eb8da303`  
		Last Modified: Sun, 27 Jun 2021 16:40:25 GMT  
		Size: 10.1 MB (10051940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca33938766a68ae61be1de59d35bcd5b4bcc18ae96c77ab8baee9b7e319e6b22`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3` - linux; s390x

```console
$ docker pull caddy@sha256:d4226a6c30e268159cbeb15e993d2320d162574b7dae654c2271619b3549bc04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14005935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f8604d50d95bbca3ab5038252554f7698f3fd2db7fbfeea946eae909416ae3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 04:05:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 26 Jun 2021 04:05:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 26 Jun 2021 04:05:30 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 26 Jun 2021 04:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_DATA_HOME=/data
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/config]
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/data]
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 26 Jun 2021 04:05:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 80
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 443
# Sat, 26 Jun 2021 04:05:42 GMT
EXPOSE 2019
# Sat, 26 Jun 2021 04:05:43 GMT
WORKDIR /srv
# Sat, 26 Jun 2021 04:05:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ffceb760cf41b73b97483b655680373ee04134e25bd41117589abadd6e8a82`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 300.8 KB (300839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e000d9bc18af630be9c570949ab0cddf3abec807b8ece78ce1d04846f41d296`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6100af0b373c529e22557cf3884882d8e6893ed368d5db1cbd63bf8529c98f6`  
		Last Modified: Sat, 26 Jun 2021 04:06:37 GMT  
		Size: 11.1 MB (11096440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce8db7df9776b5a33fa86bfa4ee4aa4f5167c8c0f5fd89be151b169616edd8`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-alpine`

```console
$ docker pull caddy@sha256:0f792d7cd96708d297fd55304917c1cad5e71b9317e68f167204d9d9e0f44657
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.3-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:77f27025e0e1e0ab97bc931db61d24f9ac41591e17576ab46c4b508afbccacd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14648199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8a741f4852592d8634aa37c7f351ae4f4e7b4a9a2594df54603ac48cbdad74`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 19:19:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 19:19:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 19:19:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 19:19:32 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 19:19:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 443
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 19:19:34 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 19:19:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d589bc046eca71df600301462981053bf178fcd31d4b2c882ca05aec70bacd`  
		Last Modified: Thu, 24 Jun 2021 19:19:59 GMT  
		Size: 11.5 MB (11529821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8ce9421f330c9a085ac8f059d2dd53feabf795c461d4f43b596d0302b1cf9`  
		Last Modified: Thu, 24 Jun 2021 19:19:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:276a06d4fac1a2986e5cade46d37a49e0954fb38a3b5ba846293c68ceef54d58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13816591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e555ad7d2e3449d758dae401706b4cc380e9747165f31c57760faa52fb6174a3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 18:50:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 24 Jun 2021 18:50:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:50:24 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:50:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:50:30 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:50:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:50:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:50:34 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:50:36 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:50:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e861f8792ad39fcefd1d13a12171eb53b6c830fc9182b96acb8bfb97c770fe4`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 300.5 KB (300519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd197178893bbfb4025a2b9c5edf60d3cd30075037c42b24c7b2b31bb8e559`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a2958808e8ef8313c312955baf1311cd2c15671f9d1ca3f59b720bd3c03ad`  
		Last Modified: Thu, 24 Jun 2021 18:52:04 GMT  
		Size: 10.9 MB (10887935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902e2228deaccfd2eec0d2ed45f03d38e9a341e018d1bacff231874d0b8b051`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:975e2acc21fa69679cd59786b1ecd7cf3d8f4ac40b028d61c219fd4e770d14cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88d5f2ec732bdfe5c5785fb90e7258f29e158c1857de067fb62436a723ec081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 04:25:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Jun 2021 04:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Fri, 25 Jun 2021 04:25:57 GMT
ENV CADDY_VERSION=v2.4.3
# Fri, 25 Jun 2021 04:26:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Jun 2021 04:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/config]
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/data]
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Jun 2021 04:26:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 80
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 443
# Fri, 25 Jun 2021 04:26:09 GMT
EXPOSE 2019
# Fri, 25 Jun 2021 04:26:09 GMT
WORKDIR /srv
# Fri, 25 Jun 2021 04:26:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532875903768e2aaa022f0dcc8d36d882e8a7af7edf14e86e6444c2406af868e`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 299.7 KB (299661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141d604c45916aa77667e44622bc085ab97eec4f8ba487d6f06aed74e53395a4`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e46c35d91cdc127af615f56a9074bd03baf63f40550c10ac1e56edf111fd4e`  
		Last Modified: Fri, 25 Jun 2021 04:27:42 GMT  
		Size: 10.9 MB (10863654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7106f92e86cc0f43d86170e3424675fb1543f58df755ce212946b44d5c96c38`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:780ee1b9ce06277bd5c34b2d9a6908cdb3028aa838fa75e5c6e1e32d2cabb417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13464756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a697a3b5305c041fd956ba80c8845676041e98bce128a69e70074e5abe9653dd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:39:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:39:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:39:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:39:33 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:39:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75403ccf5c23126b5dca334871ec0096a90d0fb85f47be1ecba3904921529c0`  
		Last Modified: Thu, 24 Jun 2021 18:40:18 GMT  
		Size: 10.4 MB (10446098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a85edeaa46fe5e0185f11a1a1801c0d0458e59897d3c04e97136df1c496663`  
		Last Modified: Thu, 24 Jun 2021 18:40:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:31130c0111ca19a1dca906ee7b2cc380f8e67ab892979cf56bb190c094f1522f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13173628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd0ea8d539e938e13773b20a1ea1796adb72671700cb9b65b480a669b6e3f8d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 16:38:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sun, 27 Jun 2021 16:38:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sun, 27 Jun 2021 16:38:15 GMT
ENV CADDY_VERSION=v2.4.3
# Sun, 27 Jun 2021 16:38:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sun, 27 Jun 2021 16:38:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sun, 27 Jun 2021 16:38:32 GMT
ENV XDG_CONFIG_HOME=/config
# Sun, 27 Jun 2021 16:38:34 GMT
ENV XDG_DATA_HOME=/data
# Sun, 27 Jun 2021 16:38:36 GMT
VOLUME [/config]
# Sun, 27 Jun 2021 16:38:40 GMT
VOLUME [/data]
# Sun, 27 Jun 2021 16:38:42 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sun, 27 Jun 2021 16:38:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Sun, 27 Jun 2021 16:38:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sun, 27 Jun 2021 16:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sun, 27 Jun 2021 16:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sun, 27 Jun 2021 16:38:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sun, 27 Jun 2021 16:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sun, 27 Jun 2021 16:38:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sun, 27 Jun 2021 16:39:01 GMT
EXPOSE 80
# Sun, 27 Jun 2021 16:39:03 GMT
EXPOSE 443
# Sun, 27 Jun 2021 16:39:07 GMT
EXPOSE 2019
# Sun, 27 Jun 2021 16:39:10 GMT
WORKDIR /srv
# Sun, 27 Jun 2021 16:39:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd997e1dce51da7846f8347657708b8750a0eb8c5e786c5fcef5547e42d3e9c`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 302.5 KB (302543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65a4be1a04251210dcf5d4925c25d6f9079b4bf699f80e43a2513e46421a5`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 5.9 KB (5851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f2bf16517247de92fb2f9a568c2775d92d15e09db858d1f639199eb8da303`  
		Last Modified: Sun, 27 Jun 2021 16:40:25 GMT  
		Size: 10.1 MB (10051940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca33938766a68ae61be1de59d35bcd5b4bcc18ae96c77ab8baee9b7e319e6b22`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d4226a6c30e268159cbeb15e993d2320d162574b7dae654c2271619b3549bc04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14005935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f8604d50d95bbca3ab5038252554f7698f3fd2db7fbfeea946eae909416ae3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 04:05:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 26 Jun 2021 04:05:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 26 Jun 2021 04:05:30 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 26 Jun 2021 04:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_DATA_HOME=/data
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/config]
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/data]
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 26 Jun 2021 04:05:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 80
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 443
# Sat, 26 Jun 2021 04:05:42 GMT
EXPOSE 2019
# Sat, 26 Jun 2021 04:05:43 GMT
WORKDIR /srv
# Sat, 26 Jun 2021 04:05:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ffceb760cf41b73b97483b655680373ee04134e25bd41117589abadd6e8a82`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 300.8 KB (300839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e000d9bc18af630be9c570949ab0cddf3abec807b8ece78ce1d04846f41d296`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6100af0b373c529e22557cf3884882d8e6893ed368d5db1cbd63bf8529c98f6`  
		Last Modified: Sat, 26 Jun 2021 04:06:37 GMT  
		Size: 11.1 MB (11096440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce8db7df9776b5a33fa86bfa4ee4aa4f5167c8c0f5fd89be151b169616edd8`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-builder`

```console
$ docker pull caddy@sha256:a67ad5e8b31cce8d525433db1ed70bcf31dadb0a6232fede113d6aa29ff6bd9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:2.4.3-builder` - linux; amd64

```console
$ docker pull caddy@sha256:f6cdd65e955bc74496559b799a16c919549831ca75ccfc32dc5ef04d1fc4e5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116854935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871368d0c2131d992e382b9e0d4ade9b0ff877237c1f08e1f0439744ae010b4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:20:03 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:20:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:20:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:29 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:44:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 00:44:31 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:44:32 GMT
WORKDIR /go
# Tue, 13 Jul 2021 22:43:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 22:43:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 22:43:41 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 22:43:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 22:43:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 22:43:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 22:43:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8dd7cab73593e079aa6f5b2fe6c2adfe09761320c162696f8fbdc9d81c99e6`  
		Last Modified: Fri, 25 Jun 2021 23:16:30 GMT  
		Size: 281.5 KB (281504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac70760d29a8ed86a3f007ed2410ef62cc877ddd2ceaa3e10806664fb3d1d1`  
		Last Modified: Fri, 25 Jun 2021 23:16:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edffed539bd83dee46e0e9cad74f38623ec3cd1cdafa538a8f390f1ce3dad86`  
		Last Modified: Tue, 13 Jul 2021 00:57:36 GMT  
		Size: 105.8 MB (105823516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4005d2dc874b23b426670e96f7fd6fb135e699c7424968915b39092a6c65413`  
		Last Modified: Tue, 13 Jul 2021 00:57:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707db5879f70d57e47f626fefe4da13194e93987052fbb6abafadb7ffdd1baf`  
		Last Modified: Tue, 13 Jul 2021 22:44:16 GMT  
		Size: 6.6 MB (6626557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692866fb377b59f86eaf10234066d2f1d916074aa34c13847cbb0caf5e69bbcd`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 1.3 MB (1311164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b20931cdefb4b7578f01983d447a9eca419f53d6587b66df256aed35a14da`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3787ea93f75ebc3f9acdcbec6135c116e5efa2a9c636444bd0c6d0ad31a3c9c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112615087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4069a24bc8333ba2b78088aca22dd8150c4f7187e4f841170e050c5c1eac3f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 22:27:47 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 25 Jun 2021 22:27:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 22:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:55:15 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:57:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:57:52 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:57:55 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:11:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:11:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:11:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:11:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:11:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:11:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:11:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59daecef61f9012ed738a38ec0c69536f19c402ec68bf2b4e41224f4691ea6`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 281.7 KB (281675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33922e4ea9c90b51975f02a97ef9af96446749dc32fec4bce4f81472d5951f4c`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db3f5706e49257fa734663b30ecab76ade215386fee8d45fbe528732c8ad236`  
		Last Modified: Tue, 13 Jul 2021 02:13:03 GMT  
		Size: 102.0 MB (102002367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cfd82c985c779e28d38d13ffdd4ce57037f731afaafa87e18fa7765ccfecfa`  
		Last Modified: Tue, 13 Jul 2021 02:11:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c454daa6f4a8717d038ea20ff8db8fb988026d0e76d710c3d33ede81f6cf`  
		Last Modified: Tue, 13 Jul 2021 03:12:33 GMT  
		Size: 6.5 MB (6484276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b99595e2bdb02f0ad02d7a5bcdedce9128a3dda75833df312c3c810d8db36`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 1.2 MB (1221671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420863b180db807f8dc3c690d70856904ed5564edad8b7c4fdcce313b5637ac8`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aff38fe0c8e1a1865b4d77f303f470dda0b940df6cd371d6902c2a65807ed46e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111530985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eaed7b8bc79805b49774a853bb94da8830a86f9891a687fb782da38eb75c9e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 17:37:55 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 24 Jun 2021 17:37:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 17:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:43 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:07:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 06:07:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:07:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:07:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:07:21 GMT
WORKDIR /go
# Tue, 13 Jul 2021 10:23:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 10:23:22 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 10:23:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 10:23:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 10:23:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 10:23:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 10:23:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b6a653704b1a4485c078013594b13c6802997d9ee3aaadab95a9f5537d90fb`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 280.8 KB (280816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d159d413b624554c6f7f204b6631e5e0ffa0d8dcaecc7c187ee02b1a3046c8d`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62dae21018e5e16e900f01a5fb7663f2b12428b921c4aa202eaa3a8d0ac325`  
		Last Modified: Tue, 13 Jul 2021 06:31:05 GMT  
		Size: 101.8 MB (101818292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d2950946468eaf7199de14481fbdaf85b1d5887fba133ca2b322a552b1432`  
		Last Modified: Tue, 13 Jul 2021 06:29:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f2d2adb1c355d81282e49ce092a2bb83ee4c9d22b5bb108f7f5c285a64cdca`  
		Last Modified: Tue, 13 Jul 2021 10:24:35 GMT  
		Size: 5.8 MB (5783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9049b6efaa99533b580d82c04dfc8ef9a5427d766dd1318dc3a197cc1c1c963c`  
		Last Modified: Tue, 13 Jul 2021 10:24:34 GMT  
		Size: 1.2 MB (1219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50232af76c17b758457793588aadd38c6893d1e444164ff0cc52a2c21175ecb5`  
		Last Modified: Tue, 13 Jul 2021 10:24:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:34954aa0c8992528f20e69e7ab2924ba4a6422c90a8368468fec8644ba863c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112071299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e9b3de118d54351f56b411cfdb409214e141f9a7f07456c84c7591a164079`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:52:32 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:52:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:51 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:43:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:43:14 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:43:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:43:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:43:16 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:42:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:42:15 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:42:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:42:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:42:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:42:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ad96702509b3443881ad70a623b6184f9936c6b4cd986694020c95f3a4441c`  
		Last Modified: Fri, 25 Jun 2021 22:11:26 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bf5f5ed4dc23e2dc33456ba3ccbef3ecabf22614e760a8f4c1e3a93a6c59b`  
		Last Modified: Fri, 25 Jun 2021 22:11:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec328162280f19fa491a9223100438095ce2a77e7b9281df21e7be3bd6a7bc4`  
		Last Modified: Tue, 13 Jul 2021 01:54:27 GMT  
		Size: 101.1 MB (101142101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19e5d43a5efe6c746a1cfa2fcf1862bcc4925567d86a5c59e84ff2e1e1e9ff`  
		Last Modified: Tue, 13 Jul 2021 01:54:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527df0ff5cb43607ace2d4f041155956865d5a96f792dde6e0bc61d933aa00`  
		Last Modified: Tue, 13 Jul 2021 03:42:55 GMT  
		Size: 6.7 MB (6735645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8330a61ff9dad4df609f84bed371e68bfc277e4f5d732ef213a7a91eb2a10c4`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fcafea7f32c7cecd033dfdc40ee8ef68a394474a4db2622e529fbf14f25bd`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:74dd51e67bac5134b07d790c2346426390de3753497b1eec9bab0824e2a77232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110953352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a48de21654c9b62f43aa4fe92a4247925e90604819de1650fdcb71d8ee8b79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Tue, 20 Jul 2021 18:17:13 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Jul 2021 18:17:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Jul 2021 18:18:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jul 2021 18:21:22 GMT
ENV GOLANG_VERSION=1.16.6
# Fri, 23 Jul 2021 04:40:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 23 Jul 2021 04:40:28 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 04:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 04:41:02 GMT
WORKDIR /go
# Sat, 24 Jul 2021 05:19:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 24 Jul 2021 05:20:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 24 Jul 2021 05:20:02 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 24 Jul 2021 05:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 24 Jul 2021 05:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 24 Jul 2021 05:20:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 24 Jul 2021 05:20:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721ce277ce9262c870e1d352522e195d85ab25af4583839398f9a01c38b3dc2e`  
		Last Modified: Fri, 23 Jul 2021 04:48:01 GMT  
		Size: 283.6 KB (283650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ebf56dbf1e11bd67d55495e34cb5c84af755e9dfcaf65988531ce52a39e5d2`  
		Last Modified: Fri, 23 Jul 2021 04:48:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8592af8ad492e633c5ab1d6aa7fff04c4cfff50cbb68ad82b016ec2a1e62bb`  
		Last Modified: Fri, 23 Jul 2021 04:49:38 GMT  
		Size: 99.6 MB (99590623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600ce69bae4413214508296d621077daf64be996fb54771a68137369cc8134b`  
		Last Modified: Fri, 23 Jul 2021 04:49:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8187500a8da9f9367453b30682a867757b6194435eea42ed2f0a45d9fc7e3bfe`  
		Last Modified: Sat, 24 Jul 2021 05:20:51 GMT  
		Size: 7.1 MB (7097373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3c9911a962be6147627de3fe9b3fd513faa943eb1ab047dd5985756ff251f`  
		Last Modified: Sat, 24 Jul 2021 05:20:50 GMT  
		Size: 1.2 MB (1170514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ad770096fea4fb91c8cd35ad172b5de002fa541d7f2fb806ce9333949d561`  
		Last Modified: Sat, 24 Jul 2021 05:20:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c1fe90d100bc65dda91fdf5bdb63f816e99fc4a9928e147d2751b3a7d9d18cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc2a6a4ddf246e8517f51a95c8d6b19ea5ce09cfe97c2dc1a044bd2df444116`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Sat, 26 Jun 2021 04:05:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 26 Jun 2021 04:05:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 26 Jun 2021 04:05:55 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Jun 2021 04:05:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 26 Jun 2021 04:05:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 26 Jun 2021 04:05:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eee054ded34b1fa082776278b24e58f3711d292231b9317ab8e3596dcade07c`  
		Last Modified: Sat, 26 Jun 2021 04:06:48 GMT  
		Size: 6.5 MB (6479052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a8988e62b4b7bdcd1f3d58ab8e59e5fa2ab7ed6eca36ccfaf85f5d18eb4f5`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 1.3 MB (1264519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038b88769d2da3d3539b44720ea6f58fe16e59cf4a2e6a92ac601da04c7a51d`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:4eb06e332fdb2d502f24125aa931d24cde59802a343c6488069fb94a54ef74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852362865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e315378f9d8c30da3455c154df8d7f7363d22371e702839e334120dca02f0d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:25:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:25:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:25:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:25:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:27:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:27:07 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:28:09 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:42:39 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:45:55 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:45:59 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 17:59:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:59:42 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 17:59:45 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:59:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:00:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:01:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c50202491861e9cc59ef0cad62ab13b4d8585699abaf13275f815b0ab53bf`  
		Last Modified: Wed, 14 Jul 2021 05:03:35 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700aac46fe704c190ed71a3f8ec8f1eca6d0fed9861862fcab96996d21678657`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce5c766a8b7a15e6b68bef29d1932c4e9cf7086c6413acfcb35b89e6363813f`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3527d984880519c45793ad5f901d15605068f0a52a819044cd79ded461f09`  
		Last Modified: Wed, 14 Jul 2021 05:03:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f16e3c9a35398857e96f60776b71b2af7e30419946307d58f942fe090b2f9`  
		Last Modified: Wed, 14 Jul 2021 05:04:02 GMT  
		Size: 25.5 MB (25460385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0876037206b7bfb610c4f7906510321d8255635221cabe7945218bd0e4d6675`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e278916db542be6afd74117c73ed9743e7cdb1de94d1928e2ba00faeff6334e`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 334.2 KB (334178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b10c3fa755eb4b8899c649883154bdfabb4d8210fd05c99501bd914ac9b731`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1c58792690c81eb4a6642c459efd28697c5ff8929b42470cee6a7e4082ee1`  
		Last Modified: Wed, 14 Jul 2021 05:06:35 GMT  
		Size: 139.4 MB (139379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1825c045e930c77550f32b2d4b24f4fa8753d0cf7020f4c51ea28af9d52b89e`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.6 KB (1575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc30c19fc7720ff29534e571e8e5a1673c2675f67c177298f208911bcbc1f96`  
		Last Modified: Wed, 14 Jul 2021 18:04:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9e2c7d361d98c4325e76790bce3765156415850f328aaae18799eca52ba3a`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6d93b9213829269ca2cb4b45b481f1143b1aecbd8def9e9cd79d2d19a666`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5897ea6c031bde10f5b5ddabe05c5f99d99f378bd12f47b9c0962b4416e20cd6`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31be288471040830a89925530422731817f7d69131073c3b77722fcf1001414`  
		Last Modified: Wed, 14 Jul 2021 18:04:52 GMT  
		Size: 1.7 MB (1723702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e061480b37961b0add8ffa998c3d22f956b4722aa569338bc029a923d3ac6`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:64455ff9cc52a6eaa711eafb2f11ebc5fa78a5f15e7c1be1e4a05d2039c5eb04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6440905132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46bc0ac245d8871ca7a2ef877724591c00e6f40eb64608a40f20e5728bdd7ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:31:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:31:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:31:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:33:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:33:36 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:35:06 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:46:08 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:49:49 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:49:53 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 18:01:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:01:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 18:01:27 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 18:01:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:03:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:03:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f667c0fc8186714bfddbd565e9cdd1dd6497e3c112f1eddb17a37d1abae30c93`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3566f190f34782035012abf2530315039000f1d137ad0098f1903a99127b3b8e`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036fdd63bb05506922a2462b2487bb4ff12b9c29097537ee7d0ca4c18cad7507`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904dd19478585c0fa1c9b4a25c5ac4560759b61f3f9e2ef0e6475729d5d482`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a50006063e099df0e3d1f22baa504b0f0de1563cd642c48340cf2a8b7152bd`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 25.4 MB (25447622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445d6d1bd7224c109fda54abaaa5909b43be941934bc54c3aff8754b852ebd`  
		Last Modified: Wed, 14 Jul 2021 05:04:20 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0187f6db85279d8f0ab2b263b47845afa4452a66c28c251f571d776001e4d300`  
		Last Modified: Wed, 14 Jul 2021 05:04:21 GMT  
		Size: 318.8 KB (318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a18e3af73fb6a22be9e13447c4dc03d831112dcc5d479c52c994c324b1bca`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b18fe05fb046103c962da798acc46523e448a87265015bd0e9870d49013e2`  
		Last Modified: Wed, 14 Jul 2021 05:07:32 GMT  
		Size: 143.8 MB (143795404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eacae5fc4eee1b8807585646451e54ef2f58b632b6d045038d647606936b8f`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9145f72acba1daf6003e68907818ef42985c05eb03e5eb0886fd4f833a7b916d`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c947cad69b975374c14de848aaa54c4a57260a151a320dbe96a6348db9a8a200`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f30145eea91938fd9fabc5f8f26fe49414b7c7807a32d8cba919c9e493f826f`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eadb657f23ec662680db8a9bc4e1ade309bf93d0203e4b1c07fccf629772aa`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0920c1f5b52107603b2811da4a1f8d4d3582979217761675db22876a07e3cd`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.7 MB (1693422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239173a5587fc73012d57cf4f1387c28f9bb618c4bb423eaa0656dce5585a5c`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-builder-alpine`

```console
$ docker pull caddy@sha256:5127c38c6131f5d14b322516c0b88e8b1a6b41acc126856a7f28a677d06b5f07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.3-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:f6cdd65e955bc74496559b799a16c919549831ca75ccfc32dc5ef04d1fc4e5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116854935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871368d0c2131d992e382b9e0d4ade9b0ff877237c1f08e1f0439744ae010b4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:20:03 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:20:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:20:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:29 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:44:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 00:44:31 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:44:32 GMT
WORKDIR /go
# Tue, 13 Jul 2021 22:43:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 22:43:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 22:43:41 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 22:43:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 22:43:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 22:43:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 22:43:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8dd7cab73593e079aa6f5b2fe6c2adfe09761320c162696f8fbdc9d81c99e6`  
		Last Modified: Fri, 25 Jun 2021 23:16:30 GMT  
		Size: 281.5 KB (281504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac70760d29a8ed86a3f007ed2410ef62cc877ddd2ceaa3e10806664fb3d1d1`  
		Last Modified: Fri, 25 Jun 2021 23:16:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edffed539bd83dee46e0e9cad74f38623ec3cd1cdafa538a8f390f1ce3dad86`  
		Last Modified: Tue, 13 Jul 2021 00:57:36 GMT  
		Size: 105.8 MB (105823516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4005d2dc874b23b426670e96f7fd6fb135e699c7424968915b39092a6c65413`  
		Last Modified: Tue, 13 Jul 2021 00:57:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707db5879f70d57e47f626fefe4da13194e93987052fbb6abafadb7ffdd1baf`  
		Last Modified: Tue, 13 Jul 2021 22:44:16 GMT  
		Size: 6.6 MB (6626557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692866fb377b59f86eaf10234066d2f1d916074aa34c13847cbb0caf5e69bbcd`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 1.3 MB (1311164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b20931cdefb4b7578f01983d447a9eca419f53d6587b66df256aed35a14da`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3787ea93f75ebc3f9acdcbec6135c116e5efa2a9c636444bd0c6d0ad31a3c9c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112615087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4069a24bc8333ba2b78088aca22dd8150c4f7187e4f841170e050c5c1eac3f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 22:27:47 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 25 Jun 2021 22:27:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 22:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:55:15 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:57:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:57:52 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:57:55 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:11:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:11:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:11:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:11:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:11:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:11:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:11:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59daecef61f9012ed738a38ec0c69536f19c402ec68bf2b4e41224f4691ea6`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 281.7 KB (281675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33922e4ea9c90b51975f02a97ef9af96446749dc32fec4bce4f81472d5951f4c`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db3f5706e49257fa734663b30ecab76ade215386fee8d45fbe528732c8ad236`  
		Last Modified: Tue, 13 Jul 2021 02:13:03 GMT  
		Size: 102.0 MB (102002367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cfd82c985c779e28d38d13ffdd4ce57037f731afaafa87e18fa7765ccfecfa`  
		Last Modified: Tue, 13 Jul 2021 02:11:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c454daa6f4a8717d038ea20ff8db8fb988026d0e76d710c3d33ede81f6cf`  
		Last Modified: Tue, 13 Jul 2021 03:12:33 GMT  
		Size: 6.5 MB (6484276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b99595e2bdb02f0ad02d7a5bcdedce9128a3dda75833df312c3c810d8db36`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 1.2 MB (1221671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420863b180db807f8dc3c690d70856904ed5564edad8b7c4fdcce313b5637ac8`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aff38fe0c8e1a1865b4d77f303f470dda0b940df6cd371d6902c2a65807ed46e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111530985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eaed7b8bc79805b49774a853bb94da8830a86f9891a687fb782da38eb75c9e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 17:37:55 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 24 Jun 2021 17:37:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 17:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:43 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:07:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 06:07:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:07:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:07:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:07:21 GMT
WORKDIR /go
# Tue, 13 Jul 2021 10:23:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 10:23:22 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 10:23:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 10:23:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 10:23:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 10:23:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 10:23:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b6a653704b1a4485c078013594b13c6802997d9ee3aaadab95a9f5537d90fb`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 280.8 KB (280816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d159d413b624554c6f7f204b6631e5e0ffa0d8dcaecc7c187ee02b1a3046c8d`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62dae21018e5e16e900f01a5fb7663f2b12428b921c4aa202eaa3a8d0ac325`  
		Last Modified: Tue, 13 Jul 2021 06:31:05 GMT  
		Size: 101.8 MB (101818292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d2950946468eaf7199de14481fbdaf85b1d5887fba133ca2b322a552b1432`  
		Last Modified: Tue, 13 Jul 2021 06:29:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f2d2adb1c355d81282e49ce092a2bb83ee4c9d22b5bb108f7f5c285a64cdca`  
		Last Modified: Tue, 13 Jul 2021 10:24:35 GMT  
		Size: 5.8 MB (5783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9049b6efaa99533b580d82c04dfc8ef9a5427d766dd1318dc3a197cc1c1c963c`  
		Last Modified: Tue, 13 Jul 2021 10:24:34 GMT  
		Size: 1.2 MB (1219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50232af76c17b758457793588aadd38c6893d1e444164ff0cc52a2c21175ecb5`  
		Last Modified: Tue, 13 Jul 2021 10:24:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:34954aa0c8992528f20e69e7ab2924ba4a6422c90a8368468fec8644ba863c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112071299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e9b3de118d54351f56b411cfdb409214e141f9a7f07456c84c7591a164079`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:52:32 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:52:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:51 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:43:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:43:14 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:43:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:43:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:43:16 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:42:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:42:15 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:42:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:42:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:42:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:42:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ad96702509b3443881ad70a623b6184f9936c6b4cd986694020c95f3a4441c`  
		Last Modified: Fri, 25 Jun 2021 22:11:26 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bf5f5ed4dc23e2dc33456ba3ccbef3ecabf22614e760a8f4c1e3a93a6c59b`  
		Last Modified: Fri, 25 Jun 2021 22:11:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec328162280f19fa491a9223100438095ce2a77e7b9281df21e7be3bd6a7bc4`  
		Last Modified: Tue, 13 Jul 2021 01:54:27 GMT  
		Size: 101.1 MB (101142101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19e5d43a5efe6c746a1cfa2fcf1862bcc4925567d86a5c59e84ff2e1e1e9ff`  
		Last Modified: Tue, 13 Jul 2021 01:54:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527df0ff5cb43607ace2d4f041155956865d5a96f792dde6e0bc61d933aa00`  
		Last Modified: Tue, 13 Jul 2021 03:42:55 GMT  
		Size: 6.7 MB (6735645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8330a61ff9dad4df609f84bed371e68bfc277e4f5d732ef213a7a91eb2a10c4`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fcafea7f32c7cecd033dfdc40ee8ef68a394474a4db2622e529fbf14f25bd`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:74dd51e67bac5134b07d790c2346426390de3753497b1eec9bab0824e2a77232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110953352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a48de21654c9b62f43aa4fe92a4247925e90604819de1650fdcb71d8ee8b79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Tue, 20 Jul 2021 18:17:13 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Jul 2021 18:17:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Jul 2021 18:18:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jul 2021 18:21:22 GMT
ENV GOLANG_VERSION=1.16.6
# Fri, 23 Jul 2021 04:40:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 23 Jul 2021 04:40:28 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 04:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 04:41:02 GMT
WORKDIR /go
# Sat, 24 Jul 2021 05:19:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 24 Jul 2021 05:20:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 24 Jul 2021 05:20:02 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 24 Jul 2021 05:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 24 Jul 2021 05:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 24 Jul 2021 05:20:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 24 Jul 2021 05:20:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721ce277ce9262c870e1d352522e195d85ab25af4583839398f9a01c38b3dc2e`  
		Last Modified: Fri, 23 Jul 2021 04:48:01 GMT  
		Size: 283.6 KB (283650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ebf56dbf1e11bd67d55495e34cb5c84af755e9dfcaf65988531ce52a39e5d2`  
		Last Modified: Fri, 23 Jul 2021 04:48:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8592af8ad492e633c5ab1d6aa7fff04c4cfff50cbb68ad82b016ec2a1e62bb`  
		Last Modified: Fri, 23 Jul 2021 04:49:38 GMT  
		Size: 99.6 MB (99590623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600ce69bae4413214508296d621077daf64be996fb54771a68137369cc8134b`  
		Last Modified: Fri, 23 Jul 2021 04:49:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8187500a8da9f9367453b30682a867757b6194435eea42ed2f0a45d9fc7e3bfe`  
		Last Modified: Sat, 24 Jul 2021 05:20:51 GMT  
		Size: 7.1 MB (7097373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3c9911a962be6147627de3fe9b3fd513faa943eb1ab047dd5985756ff251f`  
		Last Modified: Sat, 24 Jul 2021 05:20:50 GMT  
		Size: 1.2 MB (1170514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ad770096fea4fb91c8cd35ad172b5de002fa541d7f2fb806ce9333949d561`  
		Last Modified: Sat, 24 Jul 2021 05:20:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1c1fe90d100bc65dda91fdf5bdb63f816e99fc4a9928e147d2751b3a7d9d18cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc2a6a4ddf246e8517f51a95c8d6b19ea5ce09cfe97c2dc1a044bd2df444116`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Sat, 26 Jun 2021 04:05:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 26 Jun 2021 04:05:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 26 Jun 2021 04:05:55 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Jun 2021 04:05:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 26 Jun 2021 04:05:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 26 Jun 2021 04:05:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eee054ded34b1fa082776278b24e58f3711d292231b9317ab8e3596dcade07c`  
		Last Modified: Sat, 26 Jun 2021 04:06:48 GMT  
		Size: 6.5 MB (6479052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a8988e62b4b7bdcd1f3d58ab8e59e5fa2ab7ed6eca36ccfaf85f5d18eb4f5`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 1.3 MB (1264519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038b88769d2da3d3539b44720ea6f58fe16e59cf4a2e6a92ac601da04c7a51d`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:19c88ab0becc5cc1a1361c8307d1a87c8f2b9f28eff7f34a7abe19090c6cdef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `caddy:2.4.3-builder-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:4eb06e332fdb2d502f24125aa931d24cde59802a343c6488069fb94a54ef74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852362865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e315378f9d8c30da3455c154df8d7f7363d22371e702839e334120dca02f0d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:25:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:25:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:25:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:25:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:27:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:27:07 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:28:09 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:42:39 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:45:55 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:45:59 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 17:59:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:59:42 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 17:59:45 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:59:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:00:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:01:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c50202491861e9cc59ef0cad62ab13b4d8585699abaf13275f815b0ab53bf`  
		Last Modified: Wed, 14 Jul 2021 05:03:35 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700aac46fe704c190ed71a3f8ec8f1eca6d0fed9861862fcab96996d21678657`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce5c766a8b7a15e6b68bef29d1932c4e9cf7086c6413acfcb35b89e6363813f`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3527d984880519c45793ad5f901d15605068f0a52a819044cd79ded461f09`  
		Last Modified: Wed, 14 Jul 2021 05:03:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f16e3c9a35398857e96f60776b71b2af7e30419946307d58f942fe090b2f9`  
		Last Modified: Wed, 14 Jul 2021 05:04:02 GMT  
		Size: 25.5 MB (25460385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0876037206b7bfb610c4f7906510321d8255635221cabe7945218bd0e4d6675`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e278916db542be6afd74117c73ed9743e7cdb1de94d1928e2ba00faeff6334e`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 334.2 KB (334178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b10c3fa755eb4b8899c649883154bdfabb4d8210fd05c99501bd914ac9b731`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1c58792690c81eb4a6642c459efd28697c5ff8929b42470cee6a7e4082ee1`  
		Last Modified: Wed, 14 Jul 2021 05:06:35 GMT  
		Size: 139.4 MB (139379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1825c045e930c77550f32b2d4b24f4fa8753d0cf7020f4c51ea28af9d52b89e`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.6 KB (1575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc30c19fc7720ff29534e571e8e5a1673c2675f67c177298f208911bcbc1f96`  
		Last Modified: Wed, 14 Jul 2021 18:04:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9e2c7d361d98c4325e76790bce3765156415850f328aaae18799eca52ba3a`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6d93b9213829269ca2cb4b45b481f1143b1aecbd8def9e9cd79d2d19a666`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5897ea6c031bde10f5b5ddabe05c5f99d99f378bd12f47b9c0962b4416e20cd6`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31be288471040830a89925530422731817f7d69131073c3b77722fcf1001414`  
		Last Modified: Wed, 14 Jul 2021 18:04:52 GMT  
		Size: 1.7 MB (1723702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e061480b37961b0add8ffa998c3d22f956b4722aa569338bc029a923d3ac6`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f0154eaa9e2dbf0c3cdcaff8538332c786fe497522a1e2277d7bee2afa8829e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `caddy:2.4.3-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:64455ff9cc52a6eaa711eafb2f11ebc5fa78a5f15e7c1be1e4a05d2039c5eb04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6440905132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46bc0ac245d8871ca7a2ef877724591c00e6f40eb64608a40f20e5728bdd7ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:31:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:31:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:31:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:33:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:33:36 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:35:06 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:46:08 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:49:49 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:49:53 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 18:01:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:01:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 18:01:27 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 18:01:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:03:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:03:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f667c0fc8186714bfddbd565e9cdd1dd6497e3c112f1eddb17a37d1abae30c93`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3566f190f34782035012abf2530315039000f1d137ad0098f1903a99127b3b8e`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036fdd63bb05506922a2462b2487bb4ff12b9c29097537ee7d0ca4c18cad7507`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904dd19478585c0fa1c9b4a25c5ac4560759b61f3f9e2ef0e6475729d5d482`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a50006063e099df0e3d1f22baa504b0f0de1563cd642c48340cf2a8b7152bd`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 25.4 MB (25447622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445d6d1bd7224c109fda54abaaa5909b43be941934bc54c3aff8754b852ebd`  
		Last Modified: Wed, 14 Jul 2021 05:04:20 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0187f6db85279d8f0ab2b263b47845afa4452a66c28c251f571d776001e4d300`  
		Last Modified: Wed, 14 Jul 2021 05:04:21 GMT  
		Size: 318.8 KB (318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a18e3af73fb6a22be9e13447c4dc03d831112dcc5d479c52c994c324b1bca`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b18fe05fb046103c962da798acc46523e448a87265015bd0e9870d49013e2`  
		Last Modified: Wed, 14 Jul 2021 05:07:32 GMT  
		Size: 143.8 MB (143795404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eacae5fc4eee1b8807585646451e54ef2f58b632b6d045038d647606936b8f`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9145f72acba1daf6003e68907818ef42985c05eb03e5eb0886fd4f833a7b916d`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c947cad69b975374c14de848aaa54c4a57260a151a320dbe96a6348db9a8a200`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f30145eea91938fd9fabc5f8f26fe49414b7c7807a32d8cba919c9e493f826f`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eadb657f23ec662680db8a9bc4e1ade309bf93d0203e4b1c07fccf629772aa`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0920c1f5b52107603b2811da4a1f8d4d3582979217761675db22876a07e3cd`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.7 MB (1693422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239173a5587fc73012d57cf4f1387c28f9bb618c4bb423eaa0656dce5585a5c`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-windowsservercore`

```console
$ docker pull caddy@sha256:7f1035763458a1b2157ab61efe3803c97713d979fe1b486a45379ccf785b0df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:2.4.3-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.3-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-windowsservercore-1809`

```console
$ docker pull caddy@sha256:3edc19bfdb3220c2ab0cdd322296d11640a5fed6927d8623bda1b75fde4db610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `caddy:2.4.3-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.3-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:ea60a37d4cd836ad64d2085c4951355657b0593ae72734ed4fae65632a0d5a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `caddy:2.4.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:0f792d7cd96708d297fd55304917c1cad5e71b9317e68f167204d9d9e0f44657
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:77f27025e0e1e0ab97bc931db61d24f9ac41591e17576ab46c4b508afbccacd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14648199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8a741f4852592d8634aa37c7f351ae4f4e7b4a9a2594df54603ac48cbdad74`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 19:19:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 19:19:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 19:19:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 19:19:32 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 19:19:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 443
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 19:19:34 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 19:19:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d589bc046eca71df600301462981053bf178fcd31d4b2c882ca05aec70bacd`  
		Last Modified: Thu, 24 Jun 2021 19:19:59 GMT  
		Size: 11.5 MB (11529821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8ce9421f330c9a085ac8f059d2dd53feabf795c461d4f43b596d0302b1cf9`  
		Last Modified: Thu, 24 Jun 2021 19:19:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:276a06d4fac1a2986e5cade46d37a49e0954fb38a3b5ba846293c68ceef54d58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13816591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e555ad7d2e3449d758dae401706b4cc380e9747165f31c57760faa52fb6174a3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 18:50:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 24 Jun 2021 18:50:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:50:24 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:50:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:50:30 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:50:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:50:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:50:34 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:50:36 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:50:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e861f8792ad39fcefd1d13a12171eb53b6c830fc9182b96acb8bfb97c770fe4`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 300.5 KB (300519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd197178893bbfb4025a2b9c5edf60d3cd30075037c42b24c7b2b31bb8e559`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a2958808e8ef8313c312955baf1311cd2c15671f9d1ca3f59b720bd3c03ad`  
		Last Modified: Thu, 24 Jun 2021 18:52:04 GMT  
		Size: 10.9 MB (10887935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902e2228deaccfd2eec0d2ed45f03d38e9a341e018d1bacff231874d0b8b051`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:975e2acc21fa69679cd59786b1ecd7cf3d8f4ac40b028d61c219fd4e770d14cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88d5f2ec732bdfe5c5785fb90e7258f29e158c1857de067fb62436a723ec081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 04:25:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Jun 2021 04:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Fri, 25 Jun 2021 04:25:57 GMT
ENV CADDY_VERSION=v2.4.3
# Fri, 25 Jun 2021 04:26:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Jun 2021 04:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/config]
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/data]
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Jun 2021 04:26:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 80
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 443
# Fri, 25 Jun 2021 04:26:09 GMT
EXPOSE 2019
# Fri, 25 Jun 2021 04:26:09 GMT
WORKDIR /srv
# Fri, 25 Jun 2021 04:26:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532875903768e2aaa022f0dcc8d36d882e8a7af7edf14e86e6444c2406af868e`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 299.7 KB (299661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141d604c45916aa77667e44622bc085ab97eec4f8ba487d6f06aed74e53395a4`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e46c35d91cdc127af615f56a9074bd03baf63f40550c10ac1e56edf111fd4e`  
		Last Modified: Fri, 25 Jun 2021 04:27:42 GMT  
		Size: 10.9 MB (10863654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7106f92e86cc0f43d86170e3424675fb1543f58df755ce212946b44d5c96c38`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:780ee1b9ce06277bd5c34b2d9a6908cdb3028aa838fa75e5c6e1e32d2cabb417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13464756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a697a3b5305c041fd956ba80c8845676041e98bce128a69e70074e5abe9653dd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:39:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:39:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:39:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:39:33 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:39:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75403ccf5c23126b5dca334871ec0096a90d0fb85f47be1ecba3904921529c0`  
		Last Modified: Thu, 24 Jun 2021 18:40:18 GMT  
		Size: 10.4 MB (10446098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a85edeaa46fe5e0185f11a1a1801c0d0458e59897d3c04e97136df1c496663`  
		Last Modified: Thu, 24 Jun 2021 18:40:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:31130c0111ca19a1dca906ee7b2cc380f8e67ab892979cf56bb190c094f1522f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13173628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd0ea8d539e938e13773b20a1ea1796adb72671700cb9b65b480a669b6e3f8d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 16:38:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sun, 27 Jun 2021 16:38:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sun, 27 Jun 2021 16:38:15 GMT
ENV CADDY_VERSION=v2.4.3
# Sun, 27 Jun 2021 16:38:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sun, 27 Jun 2021 16:38:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sun, 27 Jun 2021 16:38:32 GMT
ENV XDG_CONFIG_HOME=/config
# Sun, 27 Jun 2021 16:38:34 GMT
ENV XDG_DATA_HOME=/data
# Sun, 27 Jun 2021 16:38:36 GMT
VOLUME [/config]
# Sun, 27 Jun 2021 16:38:40 GMT
VOLUME [/data]
# Sun, 27 Jun 2021 16:38:42 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sun, 27 Jun 2021 16:38:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Sun, 27 Jun 2021 16:38:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sun, 27 Jun 2021 16:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sun, 27 Jun 2021 16:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sun, 27 Jun 2021 16:38:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sun, 27 Jun 2021 16:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sun, 27 Jun 2021 16:38:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sun, 27 Jun 2021 16:39:01 GMT
EXPOSE 80
# Sun, 27 Jun 2021 16:39:03 GMT
EXPOSE 443
# Sun, 27 Jun 2021 16:39:07 GMT
EXPOSE 2019
# Sun, 27 Jun 2021 16:39:10 GMT
WORKDIR /srv
# Sun, 27 Jun 2021 16:39:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd997e1dce51da7846f8347657708b8750a0eb8c5e786c5fcef5547e42d3e9c`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 302.5 KB (302543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65a4be1a04251210dcf5d4925c25d6f9079b4bf699f80e43a2513e46421a5`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 5.9 KB (5851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f2bf16517247de92fb2f9a568c2775d92d15e09db858d1f639199eb8da303`  
		Last Modified: Sun, 27 Jun 2021 16:40:25 GMT  
		Size: 10.1 MB (10051940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca33938766a68ae61be1de59d35bcd5b4bcc18ae96c77ab8baee9b7e319e6b22`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d4226a6c30e268159cbeb15e993d2320d162574b7dae654c2271619b3549bc04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14005935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f8604d50d95bbca3ab5038252554f7698f3fd2db7fbfeea946eae909416ae3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 04:05:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 26 Jun 2021 04:05:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 26 Jun 2021 04:05:30 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 26 Jun 2021 04:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_DATA_HOME=/data
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/config]
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/data]
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 26 Jun 2021 04:05:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 80
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 443
# Sat, 26 Jun 2021 04:05:42 GMT
EXPOSE 2019
# Sat, 26 Jun 2021 04:05:43 GMT
WORKDIR /srv
# Sat, 26 Jun 2021 04:05:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ffceb760cf41b73b97483b655680373ee04134e25bd41117589abadd6e8a82`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 300.8 KB (300839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e000d9bc18af630be9c570949ab0cddf3abec807b8ece78ce1d04846f41d296`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6100af0b373c529e22557cf3884882d8e6893ed368d5db1cbd63bf8529c98f6`  
		Last Modified: Sat, 26 Jun 2021 04:06:37 GMT  
		Size: 11.1 MB (11096440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce8db7df9776b5a33fa86bfa4ee4aa4f5167c8c0f5fd89be151b169616edd8`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:a67ad5e8b31cce8d525433db1ed70bcf31dadb0a6232fede113d6aa29ff6bd9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:f6cdd65e955bc74496559b799a16c919549831ca75ccfc32dc5ef04d1fc4e5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116854935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871368d0c2131d992e382b9e0d4ade9b0ff877237c1f08e1f0439744ae010b4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:20:03 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:20:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:20:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:29 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:44:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 00:44:31 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:44:32 GMT
WORKDIR /go
# Tue, 13 Jul 2021 22:43:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 22:43:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 22:43:41 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 22:43:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 22:43:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 22:43:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 22:43:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8dd7cab73593e079aa6f5b2fe6c2adfe09761320c162696f8fbdc9d81c99e6`  
		Last Modified: Fri, 25 Jun 2021 23:16:30 GMT  
		Size: 281.5 KB (281504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac70760d29a8ed86a3f007ed2410ef62cc877ddd2ceaa3e10806664fb3d1d1`  
		Last Modified: Fri, 25 Jun 2021 23:16:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edffed539bd83dee46e0e9cad74f38623ec3cd1cdafa538a8f390f1ce3dad86`  
		Last Modified: Tue, 13 Jul 2021 00:57:36 GMT  
		Size: 105.8 MB (105823516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4005d2dc874b23b426670e96f7fd6fb135e699c7424968915b39092a6c65413`  
		Last Modified: Tue, 13 Jul 2021 00:57:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707db5879f70d57e47f626fefe4da13194e93987052fbb6abafadb7ffdd1baf`  
		Last Modified: Tue, 13 Jul 2021 22:44:16 GMT  
		Size: 6.6 MB (6626557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692866fb377b59f86eaf10234066d2f1d916074aa34c13847cbb0caf5e69bbcd`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 1.3 MB (1311164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b20931cdefb4b7578f01983d447a9eca419f53d6587b66df256aed35a14da`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3787ea93f75ebc3f9acdcbec6135c116e5efa2a9c636444bd0c6d0ad31a3c9c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112615087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4069a24bc8333ba2b78088aca22dd8150c4f7187e4f841170e050c5c1eac3f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 22:27:47 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 25 Jun 2021 22:27:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 22:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:55:15 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:57:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:57:52 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:57:55 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:11:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:11:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:11:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:11:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:11:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:11:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:11:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59daecef61f9012ed738a38ec0c69536f19c402ec68bf2b4e41224f4691ea6`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 281.7 KB (281675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33922e4ea9c90b51975f02a97ef9af96446749dc32fec4bce4f81472d5951f4c`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db3f5706e49257fa734663b30ecab76ade215386fee8d45fbe528732c8ad236`  
		Last Modified: Tue, 13 Jul 2021 02:13:03 GMT  
		Size: 102.0 MB (102002367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cfd82c985c779e28d38d13ffdd4ce57037f731afaafa87e18fa7765ccfecfa`  
		Last Modified: Tue, 13 Jul 2021 02:11:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c454daa6f4a8717d038ea20ff8db8fb988026d0e76d710c3d33ede81f6cf`  
		Last Modified: Tue, 13 Jul 2021 03:12:33 GMT  
		Size: 6.5 MB (6484276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b99595e2bdb02f0ad02d7a5bcdedce9128a3dda75833df312c3c810d8db36`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 1.2 MB (1221671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420863b180db807f8dc3c690d70856904ed5564edad8b7c4fdcce313b5637ac8`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aff38fe0c8e1a1865b4d77f303f470dda0b940df6cd371d6902c2a65807ed46e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111530985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eaed7b8bc79805b49774a853bb94da8830a86f9891a687fb782da38eb75c9e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 17:37:55 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 24 Jun 2021 17:37:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 17:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:43 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:07:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 06:07:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:07:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:07:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:07:21 GMT
WORKDIR /go
# Tue, 13 Jul 2021 10:23:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 10:23:22 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 10:23:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 10:23:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 10:23:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 10:23:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 10:23:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b6a653704b1a4485c078013594b13c6802997d9ee3aaadab95a9f5537d90fb`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 280.8 KB (280816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d159d413b624554c6f7f204b6631e5e0ffa0d8dcaecc7c187ee02b1a3046c8d`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62dae21018e5e16e900f01a5fb7663f2b12428b921c4aa202eaa3a8d0ac325`  
		Last Modified: Tue, 13 Jul 2021 06:31:05 GMT  
		Size: 101.8 MB (101818292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d2950946468eaf7199de14481fbdaf85b1d5887fba133ca2b322a552b1432`  
		Last Modified: Tue, 13 Jul 2021 06:29:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f2d2adb1c355d81282e49ce092a2bb83ee4c9d22b5bb108f7f5c285a64cdca`  
		Last Modified: Tue, 13 Jul 2021 10:24:35 GMT  
		Size: 5.8 MB (5783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9049b6efaa99533b580d82c04dfc8ef9a5427d766dd1318dc3a197cc1c1c963c`  
		Last Modified: Tue, 13 Jul 2021 10:24:34 GMT  
		Size: 1.2 MB (1219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50232af76c17b758457793588aadd38c6893d1e444164ff0cc52a2c21175ecb5`  
		Last Modified: Tue, 13 Jul 2021 10:24:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:34954aa0c8992528f20e69e7ab2924ba4a6422c90a8368468fec8644ba863c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112071299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e9b3de118d54351f56b411cfdb409214e141f9a7f07456c84c7591a164079`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:52:32 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:52:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:51 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:43:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:43:14 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:43:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:43:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:43:16 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:42:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:42:15 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:42:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:42:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:42:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:42:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ad96702509b3443881ad70a623b6184f9936c6b4cd986694020c95f3a4441c`  
		Last Modified: Fri, 25 Jun 2021 22:11:26 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bf5f5ed4dc23e2dc33456ba3ccbef3ecabf22614e760a8f4c1e3a93a6c59b`  
		Last Modified: Fri, 25 Jun 2021 22:11:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec328162280f19fa491a9223100438095ce2a77e7b9281df21e7be3bd6a7bc4`  
		Last Modified: Tue, 13 Jul 2021 01:54:27 GMT  
		Size: 101.1 MB (101142101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19e5d43a5efe6c746a1cfa2fcf1862bcc4925567d86a5c59e84ff2e1e1e9ff`  
		Last Modified: Tue, 13 Jul 2021 01:54:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527df0ff5cb43607ace2d4f041155956865d5a96f792dde6e0bc61d933aa00`  
		Last Modified: Tue, 13 Jul 2021 03:42:55 GMT  
		Size: 6.7 MB (6735645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8330a61ff9dad4df609f84bed371e68bfc277e4f5d732ef213a7a91eb2a10c4`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fcafea7f32c7cecd033dfdc40ee8ef68a394474a4db2622e529fbf14f25bd`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:74dd51e67bac5134b07d790c2346426390de3753497b1eec9bab0824e2a77232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110953352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a48de21654c9b62f43aa4fe92a4247925e90604819de1650fdcb71d8ee8b79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Tue, 20 Jul 2021 18:17:13 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Jul 2021 18:17:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Jul 2021 18:18:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jul 2021 18:21:22 GMT
ENV GOLANG_VERSION=1.16.6
# Fri, 23 Jul 2021 04:40:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 23 Jul 2021 04:40:28 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 04:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 04:41:02 GMT
WORKDIR /go
# Sat, 24 Jul 2021 05:19:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 24 Jul 2021 05:20:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 24 Jul 2021 05:20:02 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 24 Jul 2021 05:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 24 Jul 2021 05:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 24 Jul 2021 05:20:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 24 Jul 2021 05:20:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721ce277ce9262c870e1d352522e195d85ab25af4583839398f9a01c38b3dc2e`  
		Last Modified: Fri, 23 Jul 2021 04:48:01 GMT  
		Size: 283.6 KB (283650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ebf56dbf1e11bd67d55495e34cb5c84af755e9dfcaf65988531ce52a39e5d2`  
		Last Modified: Fri, 23 Jul 2021 04:48:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8592af8ad492e633c5ab1d6aa7fff04c4cfff50cbb68ad82b016ec2a1e62bb`  
		Last Modified: Fri, 23 Jul 2021 04:49:38 GMT  
		Size: 99.6 MB (99590623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600ce69bae4413214508296d621077daf64be996fb54771a68137369cc8134b`  
		Last Modified: Fri, 23 Jul 2021 04:49:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8187500a8da9f9367453b30682a867757b6194435eea42ed2f0a45d9fc7e3bfe`  
		Last Modified: Sat, 24 Jul 2021 05:20:51 GMT  
		Size: 7.1 MB (7097373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3c9911a962be6147627de3fe9b3fd513faa943eb1ab047dd5985756ff251f`  
		Last Modified: Sat, 24 Jul 2021 05:20:50 GMT  
		Size: 1.2 MB (1170514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ad770096fea4fb91c8cd35ad172b5de002fa541d7f2fb806ce9333949d561`  
		Last Modified: Sat, 24 Jul 2021 05:20:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c1fe90d100bc65dda91fdf5bdb63f816e99fc4a9928e147d2751b3a7d9d18cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc2a6a4ddf246e8517f51a95c8d6b19ea5ce09cfe97c2dc1a044bd2df444116`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Sat, 26 Jun 2021 04:05:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 26 Jun 2021 04:05:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 26 Jun 2021 04:05:55 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Jun 2021 04:05:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 26 Jun 2021 04:05:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 26 Jun 2021 04:05:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eee054ded34b1fa082776278b24e58f3711d292231b9317ab8e3596dcade07c`  
		Last Modified: Sat, 26 Jun 2021 04:06:48 GMT  
		Size: 6.5 MB (6479052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a8988e62b4b7bdcd1f3d58ab8e59e5fa2ab7ed6eca36ccfaf85f5d18eb4f5`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 1.3 MB (1264519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038b88769d2da3d3539b44720ea6f58fe16e59cf4a2e6a92ac601da04c7a51d`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:4eb06e332fdb2d502f24125aa931d24cde59802a343c6488069fb94a54ef74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852362865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e315378f9d8c30da3455c154df8d7f7363d22371e702839e334120dca02f0d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:25:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:25:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:25:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:25:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:27:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:27:07 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:28:09 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:42:39 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:45:55 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:45:59 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 17:59:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:59:42 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 17:59:45 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:59:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:00:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:01:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c50202491861e9cc59ef0cad62ab13b4d8585699abaf13275f815b0ab53bf`  
		Last Modified: Wed, 14 Jul 2021 05:03:35 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700aac46fe704c190ed71a3f8ec8f1eca6d0fed9861862fcab96996d21678657`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce5c766a8b7a15e6b68bef29d1932c4e9cf7086c6413acfcb35b89e6363813f`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3527d984880519c45793ad5f901d15605068f0a52a819044cd79ded461f09`  
		Last Modified: Wed, 14 Jul 2021 05:03:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f16e3c9a35398857e96f60776b71b2af7e30419946307d58f942fe090b2f9`  
		Last Modified: Wed, 14 Jul 2021 05:04:02 GMT  
		Size: 25.5 MB (25460385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0876037206b7bfb610c4f7906510321d8255635221cabe7945218bd0e4d6675`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e278916db542be6afd74117c73ed9743e7cdb1de94d1928e2ba00faeff6334e`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 334.2 KB (334178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b10c3fa755eb4b8899c649883154bdfabb4d8210fd05c99501bd914ac9b731`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1c58792690c81eb4a6642c459efd28697c5ff8929b42470cee6a7e4082ee1`  
		Last Modified: Wed, 14 Jul 2021 05:06:35 GMT  
		Size: 139.4 MB (139379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1825c045e930c77550f32b2d4b24f4fa8753d0cf7020f4c51ea28af9d52b89e`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.6 KB (1575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc30c19fc7720ff29534e571e8e5a1673c2675f67c177298f208911bcbc1f96`  
		Last Modified: Wed, 14 Jul 2021 18:04:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9e2c7d361d98c4325e76790bce3765156415850f328aaae18799eca52ba3a`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6d93b9213829269ca2cb4b45b481f1143b1aecbd8def9e9cd79d2d19a666`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5897ea6c031bde10f5b5ddabe05c5f99d99f378bd12f47b9c0962b4416e20cd6`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31be288471040830a89925530422731817f7d69131073c3b77722fcf1001414`  
		Last Modified: Wed, 14 Jul 2021 18:04:52 GMT  
		Size: 1.7 MB (1723702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e061480b37961b0add8ffa998c3d22f956b4722aa569338bc029a923d3ac6`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:64455ff9cc52a6eaa711eafb2f11ebc5fa78a5f15e7c1be1e4a05d2039c5eb04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6440905132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46bc0ac245d8871ca7a2ef877724591c00e6f40eb64608a40f20e5728bdd7ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:31:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:31:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:31:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:33:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:33:36 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:35:06 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:46:08 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:49:49 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:49:53 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 18:01:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:01:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 18:01:27 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 18:01:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:03:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:03:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f667c0fc8186714bfddbd565e9cdd1dd6497e3c112f1eddb17a37d1abae30c93`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3566f190f34782035012abf2530315039000f1d137ad0098f1903a99127b3b8e`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036fdd63bb05506922a2462b2487bb4ff12b9c29097537ee7d0ca4c18cad7507`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904dd19478585c0fa1c9b4a25c5ac4560759b61f3f9e2ef0e6475729d5d482`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a50006063e099df0e3d1f22baa504b0f0de1563cd642c48340cf2a8b7152bd`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 25.4 MB (25447622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445d6d1bd7224c109fda54abaaa5909b43be941934bc54c3aff8754b852ebd`  
		Last Modified: Wed, 14 Jul 2021 05:04:20 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0187f6db85279d8f0ab2b263b47845afa4452a66c28c251f571d776001e4d300`  
		Last Modified: Wed, 14 Jul 2021 05:04:21 GMT  
		Size: 318.8 KB (318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a18e3af73fb6a22be9e13447c4dc03d831112dcc5d479c52c994c324b1bca`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b18fe05fb046103c962da798acc46523e448a87265015bd0e9870d49013e2`  
		Last Modified: Wed, 14 Jul 2021 05:07:32 GMT  
		Size: 143.8 MB (143795404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eacae5fc4eee1b8807585646451e54ef2f58b632b6d045038d647606936b8f`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9145f72acba1daf6003e68907818ef42985c05eb03e5eb0886fd4f833a7b916d`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c947cad69b975374c14de848aaa54c4a57260a151a320dbe96a6348db9a8a200`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f30145eea91938fd9fabc5f8f26fe49414b7c7807a32d8cba919c9e493f826f`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eadb657f23ec662680db8a9bc4e1ade309bf93d0203e4b1c07fccf629772aa`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0920c1f5b52107603b2811da4a1f8d4d3582979217761675db22876a07e3cd`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.7 MB (1693422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239173a5587fc73012d57cf4f1387c28f9bb618c4bb423eaa0656dce5585a5c`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:5127c38c6131f5d14b322516c0b88e8b1a6b41acc126856a7f28a677d06b5f07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:f6cdd65e955bc74496559b799a16c919549831ca75ccfc32dc5ef04d1fc4e5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116854935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871368d0c2131d992e382b9e0d4ade9b0ff877237c1f08e1f0439744ae010b4c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:20:03 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:20:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:20:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:42:29 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 00:44:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 00:44:31 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 00:44:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 00:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 00:44:32 GMT
WORKDIR /go
# Tue, 13 Jul 2021 22:43:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 22:43:41 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 22:43:41 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 22:43:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 22:43:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 22:43:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 22:43:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8dd7cab73593e079aa6f5b2fe6c2adfe09761320c162696f8fbdc9d81c99e6`  
		Last Modified: Fri, 25 Jun 2021 23:16:30 GMT  
		Size: 281.5 KB (281504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cac70760d29a8ed86a3f007ed2410ef62cc877ddd2ceaa3e10806664fb3d1d1`  
		Last Modified: Fri, 25 Jun 2021 23:16:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edffed539bd83dee46e0e9cad74f38623ec3cd1cdafa538a8f390f1ce3dad86`  
		Last Modified: Tue, 13 Jul 2021 00:57:36 GMT  
		Size: 105.8 MB (105823516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4005d2dc874b23b426670e96f7fd6fb135e699c7424968915b39092a6c65413`  
		Last Modified: Tue, 13 Jul 2021 00:57:15 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4707db5879f70d57e47f626fefe4da13194e93987052fbb6abafadb7ffdd1baf`  
		Last Modified: Tue, 13 Jul 2021 22:44:16 GMT  
		Size: 6.6 MB (6626557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692866fb377b59f86eaf10234066d2f1d916074aa34c13847cbb0caf5e69bbcd`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 1.3 MB (1311164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57b20931cdefb4b7578f01983d447a9eca419f53d6587b66df256aed35a14da`  
		Last Modified: Tue, 13 Jul 2021 22:44:15 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3787ea93f75ebc3f9acdcbec6135c116e5efa2a9c636444bd0c6d0ad31a3c9c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112615087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4069a24bc8333ba2b78088aca22dd8150c4f7187e4f841170e050c5c1eac3f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 22:27:47 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 25 Jun 2021 22:27:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 22:27:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:55:15 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:57:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:57:52 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:57:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:57:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:57:55 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:11:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:11:23 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:11:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:11:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:11:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:11:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:11:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59daecef61f9012ed738a38ec0c69536f19c402ec68bf2b4e41224f4691ea6`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 281.7 KB (281675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33922e4ea9c90b51975f02a97ef9af96446749dc32fec4bce4f81472d5951f4c`  
		Last Modified: Fri, 25 Jun 2021 22:48:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db3f5706e49257fa734663b30ecab76ade215386fee8d45fbe528732c8ad236`  
		Last Modified: Tue, 13 Jul 2021 02:13:03 GMT  
		Size: 102.0 MB (102002367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cfd82c985c779e28d38d13ffdd4ce57037f731afaafa87e18fa7765ccfecfa`  
		Last Modified: Tue, 13 Jul 2021 02:11:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c454daa6f4a8717d038ea20ff8db8fb988026d0e76d710c3d33ede81f6cf`  
		Last Modified: Tue, 13 Jul 2021 03:12:33 GMT  
		Size: 6.5 MB (6484276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b99595e2bdb02f0ad02d7a5bcdedce9128a3dda75833df312c3c810d8db36`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 1.2 MB (1221671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420863b180db807f8dc3c690d70856904ed5564edad8b7c4fdcce313b5637ac8`  
		Last Modified: Tue, 13 Jul 2021 03:12:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:aff38fe0c8e1a1865b4d77f303f470dda0b940df6cd371d6902c2a65807ed46e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111530985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eaed7b8bc79805b49774a853bb94da8830a86f9891a687fb782da38eb75c9e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 17:37:55 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 24 Jun 2021 17:37:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 17:37:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:04:43 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:07:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 06:07:19 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:07:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:07:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:07:21 GMT
WORKDIR /go
# Tue, 13 Jul 2021 10:23:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 10:23:22 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 10:23:23 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 10:23:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 10:23:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 10:23:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 10:23:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b6a653704b1a4485c078013594b13c6802997d9ee3aaadab95a9f5537d90fb`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 280.8 KB (280816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d159d413b624554c6f7f204b6631e5e0ffa0d8dcaecc7c187ee02b1a3046c8d`  
		Last Modified: Fri, 25 Jun 2021 23:05:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62dae21018e5e16e900f01a5fb7663f2b12428b921c4aa202eaa3a8d0ac325`  
		Last Modified: Tue, 13 Jul 2021 06:31:05 GMT  
		Size: 101.8 MB (101818292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d2950946468eaf7199de14481fbdaf85b1d5887fba133ca2b322a552b1432`  
		Last Modified: Tue, 13 Jul 2021 06:29:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f2d2adb1c355d81282e49ce092a2bb83ee4c9d22b5bb108f7f5c285a64cdca`  
		Last Modified: Tue, 13 Jul 2021 10:24:35 GMT  
		Size: 5.8 MB (5783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9049b6efaa99533b580d82c04dfc8ef9a5427d766dd1318dc3a197cc1c1c963c`  
		Last Modified: Tue, 13 Jul 2021 10:24:34 GMT  
		Size: 1.2 MB (1219494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50232af76c17b758457793588aadd38c6893d1e444164ff0cc52a2c21175ecb5`  
		Last Modified: Tue, 13 Jul 2021 10:24:33 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:34954aa0c8992528f20e69e7ab2924ba4a6422c90a8368468fec8644ba863c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112071299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744e9b3de118d54351f56b411cfdb409214e141f9a7f07456c84c7591a164079`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:52:32 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 16 Jun 2021 23:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 23:52:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:41:51 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 01:43:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 13 Jul 2021 01:43:14 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 01:43:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 01:43:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 01:43:16 GMT
WORKDIR /go
# Tue, 13 Jul 2021 03:42:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 13 Jul 2021 03:42:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 13 Jul 2021 03:42:15 GMT
ENV CADDY_VERSION=v2.4.3
# Tue, 13 Jul 2021 03:42:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 13 Jul 2021 03:42:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 13 Jul 2021 03:42:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 13 Jul 2021 03:42:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ad96702509b3443881ad70a623b6184f9936c6b4cd986694020c95f3a4441c`  
		Last Modified: Fri, 25 Jun 2021 22:11:26 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bf5f5ed4dc23e2dc33456ba3ccbef3ecabf22614e760a8f4c1e3a93a6c59b`  
		Last Modified: Fri, 25 Jun 2021 22:11:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec328162280f19fa491a9223100438095ce2a77e7b9281df21e7be3bd6a7bc4`  
		Last Modified: Tue, 13 Jul 2021 01:54:27 GMT  
		Size: 101.1 MB (101142101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19e5d43a5efe6c746a1cfa2fcf1862bcc4925567d86a5c59e84ff2e1e1e9ff`  
		Last Modified: Tue, 13 Jul 2021 01:54:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93527df0ff5cb43607ace2d4f041155956865d5a96f792dde6e0bc61d933aa00`  
		Last Modified: Tue, 13 Jul 2021 03:42:55 GMT  
		Size: 6.7 MB (6735645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8330a61ff9dad4df609f84bed371e68bfc277e4f5d732ef213a7a91eb2a10c4`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fcafea7f32c7cecd033dfdc40ee8ef68a394474a4db2622e529fbf14f25bd`  
		Last Modified: Tue, 13 Jul 2021 03:42:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:74dd51e67bac5134b07d790c2346426390de3753497b1eec9bab0824e2a77232
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110953352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a48de21654c9b62f43aa4fe92a4247925e90604819de1650fdcb71d8ee8b79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Tue, 20 Jul 2021 18:17:13 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 20 Jul 2021 18:17:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Jul 2021 18:18:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Jul 2021 18:21:22 GMT
ENV GOLANG_VERSION=1.16.6
# Fri, 23 Jul 2021 04:40:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 	sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		./make.bash; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 23 Jul 2021 04:40:28 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 04:40:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:40:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 04:41:02 GMT
WORKDIR /go
# Sat, 24 Jul 2021 05:19:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 24 Jul 2021 05:20:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 24 Jul 2021 05:20:02 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 24 Jul 2021 05:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 24 Jul 2021 05:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 24 Jul 2021 05:20:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 24 Jul 2021 05:20:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721ce277ce9262c870e1d352522e195d85ab25af4583839398f9a01c38b3dc2e`  
		Last Modified: Fri, 23 Jul 2021 04:48:01 GMT  
		Size: 283.6 KB (283650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ebf56dbf1e11bd67d55495e34cb5c84af755e9dfcaf65988531ce52a39e5d2`  
		Last Modified: Fri, 23 Jul 2021 04:48:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8592af8ad492e633c5ab1d6aa7fff04c4cfff50cbb68ad82b016ec2a1e62bb`  
		Last Modified: Fri, 23 Jul 2021 04:49:38 GMT  
		Size: 99.6 MB (99590623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600ce69bae4413214508296d621077daf64be996fb54771a68137369cc8134b`  
		Last Modified: Fri, 23 Jul 2021 04:49:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8187500a8da9f9367453b30682a867757b6194435eea42ed2f0a45d9fc7e3bfe`  
		Last Modified: Sat, 24 Jul 2021 05:20:51 GMT  
		Size: 7.1 MB (7097373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3c9911a962be6147627de3fe9b3fd513faa943eb1ab047dd5985756ff251f`  
		Last Modified: Sat, 24 Jul 2021 05:20:50 GMT  
		Size: 1.2 MB (1170514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ad770096fea4fb91c8cd35ad172b5de002fa541d7f2fb806ce9333949d561`  
		Last Modified: Sat, 24 Jul 2021 05:20:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1c1fe90d100bc65dda91fdf5bdb63f816e99fc4a9928e147d2751b3a7d9d18cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bc2a6a4ddf246e8517f51a95c8d6b19ea5ce09cfe97c2dc1a044bd2df444116`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Jun 2021 01:26:42 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Sat, 26 Jun 2021 04:05:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 26 Jun 2021 04:05:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Sat, 26 Jun 2021 04:05:55 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Jun 2021 04:05:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 26 Jun 2021 04:05:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 26 Jun 2021 04:05:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eee054ded34b1fa082776278b24e58f3711d292231b9317ab8e3596dcade07c`  
		Last Modified: Sat, 26 Jun 2021 04:06:48 GMT  
		Size: 6.5 MB (6479052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a8988e62b4b7bdcd1f3d58ab8e59e5fa2ab7ed6eca36ccfaf85f5d18eb4f5`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 1.3 MB (1264519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038b88769d2da3d3539b44720ea6f58fe16e59cf4a2e6a92ac601da04c7a51d`  
		Last Modified: Sat, 26 Jun 2021 04:06:47 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:19c88ab0becc5cc1a1361c8307d1a87c8f2b9f28eff7f34a7abe19090c6cdef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:4eb06e332fdb2d502f24125aa931d24cde59802a343c6488069fb94a54ef74a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852362865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e315378f9d8c30da3455c154df8d7f7363d22371e702839e334120dca02f0d4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:25:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:25:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:25:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:25:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:27:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:27:07 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:28:09 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:42:39 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:45:55 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:45:59 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 17:59:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:59:42 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 17:59:45 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:59:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:00:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:01:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c50202491861e9cc59ef0cad62ab13b4d8585699abaf13275f815b0ab53bf`  
		Last Modified: Wed, 14 Jul 2021 05:03:35 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700aac46fe704c190ed71a3f8ec8f1eca6d0fed9861862fcab96996d21678657`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce5c766a8b7a15e6b68bef29d1932c4e9cf7086c6413acfcb35b89e6363813f`  
		Last Modified: Wed, 14 Jul 2021 05:03:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3527d984880519c45793ad5f901d15605068f0a52a819044cd79ded461f09`  
		Last Modified: Wed, 14 Jul 2021 05:03:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f16e3c9a35398857e96f60776b71b2af7e30419946307d58f942fe090b2f9`  
		Last Modified: Wed, 14 Jul 2021 05:04:02 GMT  
		Size: 25.5 MB (25460385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0876037206b7bfb610c4f7906510321d8255635221cabe7945218bd0e4d6675`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e278916db542be6afd74117c73ed9743e7cdb1de94d1928e2ba00faeff6334e`  
		Last Modified: Wed, 14 Jul 2021 05:03:30 GMT  
		Size: 334.2 KB (334178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b10c3fa755eb4b8899c649883154bdfabb4d8210fd05c99501bd914ac9b731`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1c58792690c81eb4a6642c459efd28697c5ff8929b42470cee6a7e4082ee1`  
		Last Modified: Wed, 14 Jul 2021 05:06:35 GMT  
		Size: 139.4 MB (139379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1825c045e930c77550f32b2d4b24f4fa8753d0cf7020f4c51ea28af9d52b89e`  
		Last Modified: Wed, 14 Jul 2021 05:06:00 GMT  
		Size: 1.6 KB (1575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc30c19fc7720ff29534e571e8e5a1673c2675f67c177298f208911bcbc1f96`  
		Last Modified: Wed, 14 Jul 2021 18:04:49 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9e2c7d361d98c4325e76790bce3765156415850f328aaae18799eca52ba3a`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6d93b9213829269ca2cb4b45b481f1143b1aecbd8def9e9cd79d2d19a666`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5897ea6c031bde10f5b5ddabe05c5f99d99f378bd12f47b9c0962b4416e20cd6`  
		Last Modified: Wed, 14 Jul 2021 18:04:47 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31be288471040830a89925530422731817f7d69131073c3b77722fcf1001414`  
		Last Modified: Wed, 14 Jul 2021 18:04:52 GMT  
		Size: 1.7 MB (1723702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45e061480b37961b0add8ffa998c3d22f956b4722aa569338bc029a923d3ac6`  
		Last Modified: Wed, 14 Jul 2021 18:04:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f0154eaa9e2dbf0c3cdcaff8538332c786fe497522a1e2277d7bee2afa8829e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:64455ff9cc52a6eaa711eafb2f11ebc5fa78a5f15e7c1be1e4a05d2039c5eb04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6440905132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46bc0ac245d8871ca7a2ef877724591c00e6f40eb64608a40f20e5728bdd7ae`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 04:31:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Jul 2021 04:31:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Jul 2021 04:31:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Jul 2021 04:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Jul 2021 04:33:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:33:36 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:35:06 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 04:46:08 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:49:49 GMT
RUN $url = 'https://dl.google.com/go/go1.16.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c1132ba4e6263a1712355fb0745bf4f23e1602e1661c20f071e08bdcc5fe8db5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 04:49:53 GMT
WORKDIR C:\gopath
# Wed, 14 Jul 2021 18:01:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 18:01:24 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 14 Jul 2021 18:01:27 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 18:01:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 14 Jul 2021 18:03:01 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 14 Jul 2021 18:03:04 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f667c0fc8186714bfddbd565e9cdd1dd6497e3c112f1eddb17a37d1abae30c93`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3566f190f34782035012abf2530315039000f1d137ad0098f1903a99127b3b8e`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036fdd63bb05506922a2462b2487bb4ff12b9c29097537ee7d0ca4c18cad7507`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8904dd19478585c0fa1c9b4a25c5ac4560759b61f3f9e2ef0e6475729d5d482`  
		Last Modified: Wed, 14 Jul 2021 05:04:24 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a50006063e099df0e3d1f22baa504b0f0de1563cd642c48340cf2a8b7152bd`  
		Last Modified: Wed, 14 Jul 2021 05:04:30 GMT  
		Size: 25.4 MB (25447622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445d6d1bd7224c109fda54abaaa5909b43be941934bc54c3aff8754b852ebd`  
		Last Modified: Wed, 14 Jul 2021 05:04:20 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0187f6db85279d8f0ab2b263b47845afa4452a66c28c251f571d776001e4d300`  
		Last Modified: Wed, 14 Jul 2021 05:04:21 GMT  
		Size: 318.8 KB (318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a18e3af73fb6a22be9e13447c4dc03d831112dcc5d479c52c994c324b1bca`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3b18fe05fb046103c962da798acc46523e448a87265015bd0e9870d49013e2`  
		Last Modified: Wed, 14 Jul 2021 05:07:32 GMT  
		Size: 143.8 MB (143795404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eacae5fc4eee1b8807585646451e54ef2f58b632b6d045038d647606936b8f`  
		Last Modified: Wed, 14 Jul 2021 05:06:53 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9145f72acba1daf6003e68907818ef42985c05eb03e5eb0886fd4f833a7b916d`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c947cad69b975374c14de848aaa54c4a57260a151a320dbe96a6348db9a8a200`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f30145eea91938fd9fabc5f8f26fe49414b7c7807a32d8cba919c9e493f826f`  
		Last Modified: Wed, 14 Jul 2021 18:05:06 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eadb657f23ec662680db8a9bc4e1ade309bf93d0203e4b1c07fccf629772aa`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0920c1f5b52107603b2811da4a1f8d4d3582979217761675db22876a07e3cd`  
		Last Modified: Wed, 14 Jul 2021 18:05:09 GMT  
		Size: 1.7 MB (1693422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239173a5587fc73012d57cf4f1387c28f9bb618c4bb423eaa0656dce5585a5c`  
		Last Modified: Wed, 14 Jul 2021 18:05:07 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:90dfeaa3846391a67e0e9dec49fbe8c3031eec18cdbb92258b2e45bcd1c775d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:77f27025e0e1e0ab97bc931db61d24f9ac41591e17576ab46c4b508afbccacd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14648199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8a741f4852592d8634aa37c7f351ae4f4e7b4a9a2594df54603ac48cbdad74`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 19:19:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 19:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 19:19:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 19:19:31 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 19:19:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 19:19:32 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 19:19:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 19:19:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 19:19:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 443
# Thu, 24 Jun 2021 19:19:34 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 19:19:34 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 19:19:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d589bc046eca71df600301462981053bf178fcd31d4b2c882ca05aec70bacd`  
		Last Modified: Thu, 24 Jun 2021 19:19:59 GMT  
		Size: 11.5 MB (11529821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8ce9421f330c9a085ac8f059d2dd53feabf795c461d4f43b596d0302b1cf9`  
		Last Modified: Thu, 24 Jun 2021 19:19:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:276a06d4fac1a2986e5cade46d37a49e0954fb38a3b5ba846293c68ceef54d58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13816591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e555ad7d2e3449d758dae401706b4cc380e9747165f31c57760faa52fb6174a3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 18:50:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 24 Jun 2021 18:50:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:50:24 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:50:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:50:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:50:30 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:50:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:50:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:50:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:50:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:50:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:50:34 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:50:35 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:50:36 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:50:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e861f8792ad39fcefd1d13a12171eb53b6c830fc9182b96acb8bfb97c770fe4`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 300.5 KB (300519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd197178893bbfb4025a2b9c5edf60d3cd30075037c42b24c7b2b31bb8e559`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a2958808e8ef8313c312955baf1311cd2c15671f9d1ca3f59b720bd3c03ad`  
		Last Modified: Thu, 24 Jun 2021 18:52:04 GMT  
		Size: 10.9 MB (10887935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902e2228deaccfd2eec0d2ed45f03d38e9a341e018d1bacff231874d0b8b051`  
		Last Modified: Thu, 24 Jun 2021 18:51:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:975e2acc21fa69679cd59786b1ecd7cf3d8f4ac40b028d61c219fd4e770d14cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88d5f2ec732bdfe5c5785fb90e7258f29e158c1857de067fb62436a723ec081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 04:25:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Jun 2021 04:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Fri, 25 Jun 2021 04:25:57 GMT
ENV CADDY_VERSION=v2.4.3
# Fri, 25 Jun 2021 04:26:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Jun 2021 04:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Jun 2021 04:26:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/config]
# Fri, 25 Jun 2021 04:26:04 GMT
VOLUME [/data]
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Jun 2021 04:26:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Jun 2021 04:26:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Jun 2021 04:26:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Jun 2021 04:26:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 80
# Fri, 25 Jun 2021 04:26:08 GMT
EXPOSE 443
# Fri, 25 Jun 2021 04:26:09 GMT
EXPOSE 2019
# Fri, 25 Jun 2021 04:26:09 GMT
WORKDIR /srv
# Fri, 25 Jun 2021 04:26:10 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532875903768e2aaa022f0dcc8d36d882e8a7af7edf14e86e6444c2406af868e`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 299.7 KB (299661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141d604c45916aa77667e44622bc085ab97eec4f8ba487d6f06aed74e53395a4`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e46c35d91cdc127af615f56a9074bd03baf63f40550c10ac1e56edf111fd4e`  
		Last Modified: Fri, 25 Jun 2021 04:27:42 GMT  
		Size: 10.9 MB (10863654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7106f92e86cc0f43d86170e3424675fb1543f58df755ce212946b44d5c96c38`  
		Last Modified: Fri, 25 Jun 2021 04:27:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:780ee1b9ce06277bd5c34b2d9a6908cdb3028aa838fa75e5c6e1e32d2cabb417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13464756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a697a3b5305c041fd956ba80c8845676041e98bce128a69e70074e5abe9653dd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Thu, 24 Jun 2021 18:39:27 GMT
ENV CADDY_VERSION=v2.4.3
# Thu, 24 Jun 2021 18:39:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 24 Jun 2021 18:39:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 24 Jun 2021 18:39:30 GMT
ENV XDG_DATA_HOME=/data
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/config]
# Thu, 24 Jun 2021 18:39:31 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 24 Jun 2021 18:39:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 24 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 80
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 443
# Thu, 24 Jun 2021 18:39:33 GMT
EXPOSE 2019
# Thu, 24 Jun 2021 18:39:33 GMT
WORKDIR /srv
# Thu, 24 Jun 2021 18:39:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75403ccf5c23126b5dca334871ec0096a90d0fb85f47be1ecba3904921529c0`  
		Last Modified: Thu, 24 Jun 2021 18:40:18 GMT  
		Size: 10.4 MB (10446098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a85edeaa46fe5e0185f11a1a1801c0d0458e59897d3c04e97136df1c496663`  
		Last Modified: Thu, 24 Jun 2021 18:40:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:31130c0111ca19a1dca906ee7b2cc380f8e67ab892979cf56bb190c094f1522f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13173628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd0ea8d539e938e13773b20a1ea1796adb72671700cb9b65b480a669b6e3f8d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 16:38:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sun, 27 Jun 2021 16:38:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sun, 27 Jun 2021 16:38:15 GMT
ENV CADDY_VERSION=v2.4.3
# Sun, 27 Jun 2021 16:38:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sun, 27 Jun 2021 16:38:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sun, 27 Jun 2021 16:38:32 GMT
ENV XDG_CONFIG_HOME=/config
# Sun, 27 Jun 2021 16:38:34 GMT
ENV XDG_DATA_HOME=/data
# Sun, 27 Jun 2021 16:38:36 GMT
VOLUME [/config]
# Sun, 27 Jun 2021 16:38:40 GMT
VOLUME [/data]
# Sun, 27 Jun 2021 16:38:42 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sun, 27 Jun 2021 16:38:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Sun, 27 Jun 2021 16:38:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sun, 27 Jun 2021 16:38:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sun, 27 Jun 2021 16:38:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sun, 27 Jun 2021 16:38:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sun, 27 Jun 2021 16:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sun, 27 Jun 2021 16:38:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sun, 27 Jun 2021 16:39:01 GMT
EXPOSE 80
# Sun, 27 Jun 2021 16:39:03 GMT
EXPOSE 443
# Sun, 27 Jun 2021 16:39:07 GMT
EXPOSE 2019
# Sun, 27 Jun 2021 16:39:10 GMT
WORKDIR /srv
# Sun, 27 Jun 2021 16:39:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd997e1dce51da7846f8347657708b8750a0eb8c5e786c5fcef5547e42d3e9c`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 302.5 KB (302543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd65a4be1a04251210dcf5d4925c25d6f9079b4bf699f80e43a2513e46421a5`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 5.9 KB (5851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f2bf16517247de92fb2f9a568c2775d92d15e09db858d1f639199eb8da303`  
		Last Modified: Sun, 27 Jun 2021 16:40:25 GMT  
		Size: 10.1 MB (10051940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca33938766a68ae61be1de59d35bcd5b4bcc18ae96c77ab8baee9b7e319e6b22`  
		Last Modified: Sun, 27 Jun 2021 16:40:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:d4226a6c30e268159cbeb15e993d2320d162574b7dae654c2271619b3549bc04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14005935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f8604d50d95bbca3ab5038252554f7698f3fd2db7fbfeea946eae909416ae3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 04:05:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 26 Jun 2021 04:05:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Sat, 26 Jun 2021 04:05:30 GMT
ENV CADDY_VERSION=v2.4.3
# Sat, 26 Jun 2021 04:05:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1b39843c198a56ccaf1af19edfe51ff2556d6c9081cbf52bbf8d697777af936b24e872561ca0b35aafa0c84b05c86faa4c2ccf463ffef31bb7140fd09211595c' ;; 		armhf)   binArch='armv6'; checksum='9a1e606bbb6d965ab92b7bcae6a5b58fbffa7f9bec77be3321509e3175e18c8f9db785af40e91bc570f799ea9c44756ff0694439a0b4d30574ea50eee7854693' ;; 		armv7)   binArch='armv7'; checksum='67c1af278bfb79daaf7a2717206b94e09ebfac433c5ce8ef2bad1e1233d626c5b57e822a0c29205b7c62561a06772f116d7dcf072ebea4b3148f0bbaa2f61f6c' ;; 		aarch64) binArch='arm64'; checksum='fa105a900a21f02175a1ab1ff2d0db4f171832183f231d59f265d3f728ac9ec7ff4f2b2a951dccf8f6d7a7057fc69e5670db18bd150ff5bd63df3f72c81cff39' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='71399082625f3059208e590b5d13c700757bcb077063115f26f257ab83b3c51d35eabcf70f0cfb426cb5cb59193ee15301dc2f35b22d2d23f6cf8678c84462a6' ;; 		s390x)   binArch='s390x'; checksum='96c9bcb89fb1083c3a293ccc3568b58fc64cfcfda4983fd244a20be07b1b5e26b54bf155d0e472f035d584f1484bd17073c27a75b72adac7d3a820a616015887' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 26 Jun 2021 04:05:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 26 Jun 2021 04:05:36 GMT
ENV XDG_DATA_HOME=/data
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/config]
# Sat, 26 Jun 2021 04:05:37 GMT
VOLUME [/data]
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 26 Jun 2021 04:05:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 26 Jun 2021 04:05:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 26 Jun 2021 04:05:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 26 Jun 2021 04:05:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 80
# Sat, 26 Jun 2021 04:05:41 GMT
EXPOSE 443
# Sat, 26 Jun 2021 04:05:42 GMT
EXPOSE 2019
# Sat, 26 Jun 2021 04:05:43 GMT
WORKDIR /srv
# Sat, 26 Jun 2021 04:05:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ffceb760cf41b73b97483b655680373ee04134e25bd41117589abadd6e8a82`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 300.8 KB (300839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e000d9bc18af630be9c570949ab0cddf3abec807b8ece78ce1d04846f41d296`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6100af0b373c529e22557cf3884882d8e6893ed368d5db1cbd63bf8529c98f6`  
		Last Modified: Sat, 26 Jun 2021 04:06:37 GMT  
		Size: 11.1 MB (11096440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce8db7df9776b5a33fa86bfa4ee4aa4f5167c8c0f5fd89be151b169616edd8`  
		Last Modified: Sat, 26 Jun 2021 04:06:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:7f1035763458a1b2157ab61efe3803c97713d979fe1b486a45379ccf785b0df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:3edc19bfdb3220c2ab0cdd322296d11640a5fed6927d8623bda1b75fde4db610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull caddy@sha256:3301868223ae5daf27b656a94db1f03025b28ecdd354036044601af9b088960a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698185366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7ab193f786384327a5517e5c86366513c0601e1e55b23f80b8d4d73c4715b4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:51:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:51:14 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:52:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:52:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:52:30 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:52:33 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:52:36 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:52:39 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:52:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:52:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:52:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:52:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:52:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:52:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:53:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:53:03 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:53:06 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:53:09 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:54:09 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:54:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61c72abd0588c9f4bcb65abaea4a08980c9cc3a10b78d6f5eaf9be83320c2e8`  
		Last Modified: Wed, 14 Jul 2021 18:03:52 GMT  
		Size: 382.8 KB (382812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec23b585668780bb01af3b50c4c7323944adede2af714b66e6bc714a9215ea`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60434d110d22fcb39f7cc361150a1717460238060b9644f8f80de76381c1b42`  
		Last Modified: Wed, 14 Jul 2021 18:03:54 GMT  
		Size: 12.0 MB (12018501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f98fcd71e884b13898d6b3b5de2cccc1a3f076024b95ffa522b041df836500`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf35d3d3dfa73a7bad7f6eaaf32f9702488d826763a7e22770c686ef8a6b865`  
		Last Modified: Wed, 14 Jul 2021 18:03:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2343de307f305b5fa42dc1bae57b7285679d58b12b58aeca26e3ce8f1dbb`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3517463a20047473a989cebd9a8c56cf5289a286453eaec6183c3f8efd76f5de`  
		Last Modified: Wed, 14 Jul 2021 18:03:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ade0652559d47e4e504b3634c5f882740f8b9a310d133a2c9426cb1d7368d1`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f74d9ad37be13f74896779e281cd290141f3231875a2141345a4b7158f96`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db73b38e7db6b8e40fa604e5aac073087f02e578f41e4c5267427ee1e1917e`  
		Last Modified: Wed, 14 Jul 2021 18:03:48 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41a9f50a8df3fd9b59f538041617403dea50fc22c3bdb1b258700a95865573`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bd865acc17f2c9b920f703eb1d73547ec7dfbbb77288fa565c0ab70bc7235`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837e6b00ba56e49374a718afddb28b17db30e4d2c908299171df8f87b2218f5`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfa12403bafd605dce611762013dc8653a664b770c2279efe8a7c15bf980a1`  
		Last Modified: Wed, 14 Jul 2021 18:03:45 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472765d102555b9aee739b1e1fed8b2cfc6bee735d516fd8f0335361e438e086`  
		Last Modified: Wed, 14 Jul 2021 18:03:46 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51d1bfe015d8f841732654d9a6bd28624566415a3810ae006e501fd23e99f1`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5690230e16d76dde7422e42d746f97650856bddd9feb4bff585fbf2a162216`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7bf00b196492eb1818026804497e6c6bc83a4b60b9585e80a62a12e2a4569f`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264976fed7db51923c9fe5872c6cc4a87fa79d4b2cbf9edea319edd0d484b631`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 311.9 KB (311910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b2c502a6cf232df0f724017ce1337897cf67cd850db31e12f5aa57f9c57a4`  
		Last Modified: Wed, 14 Jul 2021 18:03:43 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:ea60a37d4cd836ad64d2085c4951355657b0593ae72734ed4fae65632a0d5a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull caddy@sha256:bb0c7b5f47048935ba4f19d0c50f077a55808b26054d949eb43de520cc831325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282340465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc37d674fddb51ea1ea283e570fcdf6ffd759df69cce3e04b4aa21d7c65caa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 17:55:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 14 Jul 2021 17:55:52 GMT
ENV CADDY_VERSION=v2.4.3
# Wed, 14 Jul 2021 17:57:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.3/caddy_2.4.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e4b392d1384a02863f93c0e183c50a2b28a19ccf468c186fa1524b041895c237dbb88b0dd20c13d187779c0b5f5789458c84ffbc17cd628a9fd05779eb418563')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 14 Jul 2021 17:57:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 14 Jul 2021 17:57:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 14 Jul 2021 17:57:40 GMT
VOLUME [c:/config]
# Wed, 14 Jul 2021 17:57:43 GMT
VOLUME [c:/data]
# Wed, 14 Jul 2021 17:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.3
# Wed, 14 Jul 2021 17:57:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Jul 2021 17:57:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Jul 2021 17:57:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Jul 2021 17:57:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Jul 2021 17:58:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Jul 2021 17:58:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Jul 2021 17:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Jul 2021 17:58:11 GMT
EXPOSE 80
# Wed, 14 Jul 2021 17:58:13 GMT
EXPOSE 443
# Wed, 14 Jul 2021 17:58:17 GMT
EXPOSE 2019
# Wed, 14 Jul 2021 17:59:27 GMT
RUN caddy version
# Wed, 14 Jul 2021 17:59:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06238427c9b88265ed3cdfeec77aec8e724c862b5cad74b4c915f1155503fc23`  
		Last Modified: Wed, 14 Jul 2021 18:04:18 GMT  
		Size: 368.9 KB (368868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec631ec6104314fab092109f82e03e92a263f37016f9777f38216c398c0aaf21`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71310a3dc2b1ff4839f83b7fa572580cbef410952e37e7ee82b775c53d2ce630`  
		Last Modified: Wed, 14 Jul 2021 18:04:31 GMT  
		Size: 12.0 MB (12037024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8ec887f9fda7c360451ca6bcccb940af9d1a24bb69e85a3ef346ba13415d2d`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffdfdd78569260947f2b1e29f82db6de5cb5ade25556346e86db7167cfc65f`  
		Last Modified: Wed, 14 Jul 2021 18:04:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b9ff736282e8509a54b0dad98e757e205f7be0b8520be831664a5cb74bb03`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed1bfbe3cacc8f61a484038719184291148d04f84e6d2b695c1e996528e224c`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c028396699085481f6601f2f95a0f1cbba44772397c6ae19d8a0d493763b873`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35807ddc6d27e3a2a8ef0e94b444003b2fc474dd12b15f6624ae793bf2513706`  
		Last Modified: Wed, 14 Jul 2021 18:04:15 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c7dfba943a088b8b4f1517984d002b759aca03f254651e670d1d8007f0c357`  
		Last Modified: Wed, 14 Jul 2021 18:04:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428ea97e0cf35bda688dc6f8dc66673365775aeb879c6dd81d1d6f6315ca5cc`  
		Last Modified: Wed, 14 Jul 2021 18:04:13 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab24fa6fdce2f9d78ffaaf1290dd6568e8e516d949135456eaa12e70405a784`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89889237f657b2b38fa13dda844b3fd82fae1774030c2c14b30d0c53a692f896`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7322cb2537ea3d616a9a37befcae8fa41d99b2a8c0bbc92cbec5bca1b7ab`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91f62e712f8a5a941d3f050509ae2295e72d857e96917edd85d697d8474ed84`  
		Last Modified: Wed, 14 Jul 2021 18:04:12 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d552982e783bd6b630354fac745cb1870f925adb21cbe45e89af6bc51b8e6`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e980d5e293cda7f98db180869a0475da445f60e40c19c7f97e1fda93b70cc36e`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24b50f7f57376e17491201f7a792835873d08a9c2fc69c0a7316bff05dfbe9`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012676c281bbdde57c6b77b5b5774d1c1851bb2db516b2e92186d26e021be89f`  
		Last Modified: Wed, 14 Jul 2021 18:04:10 GMT  
		Size: 277.2 KB (277246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bcd309d2e58353362132147ed6353bf043d6db571b9fac67b0cc27ce26e533`  
		Last Modified: Wed, 14 Jul 2021 18:04:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
