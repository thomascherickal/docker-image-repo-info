<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2022`](#caddy2-builder-windowsservercore-ltsc2022)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2022`](#caddy2-windowsservercore-ltsc2022)
-	[`caddy:2.6.1`](#caddy261)
-	[`caddy:2.6.1-alpine`](#caddy261-alpine)
-	[`caddy:2.6.1-builder`](#caddy261-builder)
-	[`caddy:2.6.1-builder-alpine`](#caddy261-builder-alpine)
-	[`caddy:2.6.1-builder-windowsservercore-1809`](#caddy261-builder-windowsservercore-1809)
-	[`caddy:2.6.1-builder-windowsservercore-ltsc2022`](#caddy261-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6.1-windowsservercore`](#caddy261-windowsservercore)
-	[`caddy:2.6.1-windowsservercore-1809`](#caddy261-windowsservercore-1809)
-	[`caddy:2.6.1-windowsservercore-ltsc2022`](#caddy261-windowsservercore-ltsc2022)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:builder-windowsservercore-ltsc2022`](#caddybuilder-windowsservercore-ltsc2022)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2022`](#caddywindowsservercore-ltsc2022)

## `caddy:2`

```console
$ docker pull caddy@sha256:3f766f2dc97b6440bb6dcc8f105279999c60d6e0382403d7ab3be51329a692cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:5e68e231a2fb583cc2bafe472844495cd9c1b119b626cb61777a75f990886906
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181f13e1cc5fd90d0b4869e57689b5200589ca1029971fc7233082c04806a55b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 04:34:57 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:34:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 04:34:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 04:35:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 04:35:01 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 04:35:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890b94b17a6b1f257ddec10a103ff342db99516b0d339260623d6610db9b1349`  
		Last Modified: Fri, 07 Oct 2022 04:35:27 GMT  
		Size: 14.5 MB (14493818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d852ea4bd9f60570e83e432bcb361e0400dc3b2c3a264a447dfc2f6b292c0a`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:12eface0625a91f60ec1e6f8ccd864d52c9dc69f3b02ea126e4fdaacf8de5bd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0d4211357adf7a3124613f982947e3745803a9205db56b524ae70f1f03f521`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 04:09:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 08 Oct 2022 04:09:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Sat, 08 Oct 2022 04:09:55 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:09:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 08 Oct 2022 04:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 80
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443/udp
# Sat, 08 Oct 2022 04:10:00 GMT
EXPOSE 2019
# Sat, 08 Oct 2022 04:10:00 GMT
WORKDIR /srv
# Sat, 08 Oct 2022 04:10:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa0e79d89709c451dcc1ed2799b94c19204fb58ea7cce7895eef1f51c01bb50`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 304.5 KB (304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9215626c7fc1bfbffb15114b3a5de7fc64de1e7a2a21ee2056121f5ef65b2338`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ca8b546a2bb8c3467ac3eafdca5479dd6396e518b348315a1b16a18519b61`  
		Last Modified: Sat, 08 Oct 2022 04:10:49 GMT  
		Size: 13.8 MB (13848654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e20fa1676a89097bb7bfd9deb83ec1b2ba35972a2c365e7e0b111bf46a430`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8c5c01339078f89f85a5a7cd08d8bd89962900d295af83cc0eb70de31c4d51ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c275d9a5ca87dde16a12a6d524b9a542b9e77e96ead14f8c577857b6091f24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:17:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:17:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:17:46 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:17:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:17:52 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:17:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11d99bb68cba432782c86e461f4c830d8bc08ba0b2df2999db3ab67a55f57e`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 303.6 KB (303619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30dd3a0b20a2d25c12f53bf9ae92037f177e924b7613dbbeedca0029d44215`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0645b8aab72e227505345e7745508a1f23ed2ff304884458f31d828eac843`  
		Last Modified: Fri, 07 Oct 2022 07:18:46 GMT  
		Size: 13.8 MB (13824551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978d7d8e43141c7a175739d7aafcb64b5b8f6561efb3295d91c186bfab20eb3`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e6d1ad533fd36cd36a387471e708740876c809760795f8868490beab7d98443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1814d3a7f6c971e84b565c46272fc51961c9e67e0e8787781be733c087a22`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 08:00:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 08:00:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 08:00:59 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 08:01:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 08:01:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 08:01:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 08:01:06 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 08:01:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 08:01:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 08:01:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 08:01:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 08:01:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 08:01:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 08:01:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 08:01:14 GMT
EXPOSE 80
# Fri, 07 Oct 2022 08:01:15 GMT
EXPOSE 443
# Fri, 07 Oct 2022 08:01:16 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 08:01:17 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 08:01:18 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 08:01:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6fca9d7511cb60edf3b5df387d6b1fd5aaac17867575fc733cf40137b95a90`  
		Last Modified: Fri, 07 Oct 2022 08:02:04 GMT  
		Size: 304.3 KB (304303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8483ebae1fd52b4e5a413ddd322fedfc3978bd5f95dfd62ea2c53f1a0b7a7e05`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ad12dc08ecd5447289e06895740be336d526d7bec274b5cab707b3be6c4df`  
		Last Modified: Fri, 07 Oct 2022 08:02:05 GMT  
		Size: 13.2 MB (13196260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b783a84a1d985b8c4d150880a665dffed5e8d3cd282ed0f45af0b28e45c30a`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:3c296624df3a6ffb31e3a5eca10b509c80150fe12e9b19ebf27e061189d44278
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4250b6ab2344a47d567b072f8080c8f6aa93b04bd773b51fa57148ac08e30379`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:56:13 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:56:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:56:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:56:22 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:56:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d070e557e928b65136b4bb037dd73ddfb5be784310db1f0f3640ce1216afc`  
		Last Modified: Fri, 07 Oct 2022 07:57:11 GMT  
		Size: 12.9 MB (12853693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40adebe65a7cbe002c94177299a2ae8a216f554d7d6ae5eec0916ba7330da421`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:3e5aa9861d4d5e9c0dfda105fa0b598ee20d5f254b734f5a418c99f6a5b9b5af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2a3441daa59cefaa1dbb6d0edd094f53abe4b3c89877fd3b7121dd53d15ef3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 10:23:51 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:23:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 10:24:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 10:24:04 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 10:24:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 10:24:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 10:24:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 10:24:09 GMT
EXPOSE 80
# Fri, 07 Oct 2022 10:24:10 GMT
EXPOSE 443
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 10:24:12 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 10:24:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8c37b8106cb4218c6396b95deabef48406b60274cd3304a53e50b645cd9e7`  
		Last Modified: Fri, 07 Oct 2022 10:25:13 GMT  
		Size: 14.0 MB (14001566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334954d04c67d43f4bab0b7774053bae33c535a25cc073cf20528174bf6031e9`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:75d2e29d0c3ec9aa78e640c022d5afec48c2c8ccefe0f956280f66bcced7cceb
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
$ docker pull caddy@sha256:5e68e231a2fb583cc2bafe472844495cd9c1b119b626cb61777a75f990886906
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181f13e1cc5fd90d0b4869e57689b5200589ca1029971fc7233082c04806a55b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 04:34:57 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:34:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 04:34:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 04:35:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 04:35:01 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 04:35:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890b94b17a6b1f257ddec10a103ff342db99516b0d339260623d6610db9b1349`  
		Last Modified: Fri, 07 Oct 2022 04:35:27 GMT  
		Size: 14.5 MB (14493818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d852ea4bd9f60570e83e432bcb361e0400dc3b2c3a264a447dfc2f6b292c0a`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:12eface0625a91f60ec1e6f8ccd864d52c9dc69f3b02ea126e4fdaacf8de5bd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0d4211357adf7a3124613f982947e3745803a9205db56b524ae70f1f03f521`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 04:09:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 08 Oct 2022 04:09:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Sat, 08 Oct 2022 04:09:55 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:09:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 08 Oct 2022 04:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 80
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443/udp
# Sat, 08 Oct 2022 04:10:00 GMT
EXPOSE 2019
# Sat, 08 Oct 2022 04:10:00 GMT
WORKDIR /srv
# Sat, 08 Oct 2022 04:10:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa0e79d89709c451dcc1ed2799b94c19204fb58ea7cce7895eef1f51c01bb50`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 304.5 KB (304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9215626c7fc1bfbffb15114b3a5de7fc64de1e7a2a21ee2056121f5ef65b2338`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ca8b546a2bb8c3467ac3eafdca5479dd6396e518b348315a1b16a18519b61`  
		Last Modified: Sat, 08 Oct 2022 04:10:49 GMT  
		Size: 13.8 MB (13848654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e20fa1676a89097bb7bfd9deb83ec1b2ba35972a2c365e7e0b111bf46a430`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8c5c01339078f89f85a5a7cd08d8bd89962900d295af83cc0eb70de31c4d51ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c275d9a5ca87dde16a12a6d524b9a542b9e77e96ead14f8c577857b6091f24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:17:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:17:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:17:46 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:17:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:17:52 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:17:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11d99bb68cba432782c86e461f4c830d8bc08ba0b2df2999db3ab67a55f57e`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 303.6 KB (303619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30dd3a0b20a2d25c12f53bf9ae92037f177e924b7613dbbeedca0029d44215`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0645b8aab72e227505345e7745508a1f23ed2ff304884458f31d828eac843`  
		Last Modified: Fri, 07 Oct 2022 07:18:46 GMT  
		Size: 13.8 MB (13824551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978d7d8e43141c7a175739d7aafcb64b5b8f6561efb3295d91c186bfab20eb3`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e6d1ad533fd36cd36a387471e708740876c809760795f8868490beab7d98443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1814d3a7f6c971e84b565c46272fc51961c9e67e0e8787781be733c087a22`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 08:00:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 08:00:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 08:00:59 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 08:01:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 08:01:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 08:01:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 08:01:06 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 08:01:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 08:01:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 08:01:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 08:01:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 08:01:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 08:01:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 08:01:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 08:01:14 GMT
EXPOSE 80
# Fri, 07 Oct 2022 08:01:15 GMT
EXPOSE 443
# Fri, 07 Oct 2022 08:01:16 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 08:01:17 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 08:01:18 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 08:01:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6fca9d7511cb60edf3b5df387d6b1fd5aaac17867575fc733cf40137b95a90`  
		Last Modified: Fri, 07 Oct 2022 08:02:04 GMT  
		Size: 304.3 KB (304303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8483ebae1fd52b4e5a413ddd322fedfc3978bd5f95dfd62ea2c53f1a0b7a7e05`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ad12dc08ecd5447289e06895740be336d526d7bec274b5cab707b3be6c4df`  
		Last Modified: Fri, 07 Oct 2022 08:02:05 GMT  
		Size: 13.2 MB (13196260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b783a84a1d985b8c4d150880a665dffed5e8d3cd282ed0f45af0b28e45c30a`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:3c296624df3a6ffb31e3a5eca10b509c80150fe12e9b19ebf27e061189d44278
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4250b6ab2344a47d567b072f8080c8f6aa93b04bd773b51fa57148ac08e30379`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:56:13 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:56:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:56:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:56:22 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:56:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d070e557e928b65136b4bb037dd73ddfb5be784310db1f0f3640ce1216afc`  
		Last Modified: Fri, 07 Oct 2022 07:57:11 GMT  
		Size: 12.9 MB (12853693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40adebe65a7cbe002c94177299a2ae8a216f554d7d6ae5eec0916ba7330da421`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3e5aa9861d4d5e9c0dfda105fa0b598ee20d5f254b734f5a418c99f6a5b9b5af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2a3441daa59cefaa1dbb6d0edd094f53abe4b3c89877fd3b7121dd53d15ef3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 10:23:51 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:23:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 10:24:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 10:24:04 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 10:24:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 10:24:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 10:24:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 10:24:09 GMT
EXPOSE 80
# Fri, 07 Oct 2022 10:24:10 GMT
EXPOSE 443
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 10:24:12 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 10:24:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8c37b8106cb4218c6396b95deabef48406b60274cd3304a53e50b645cd9e7`  
		Last Modified: Fri, 07 Oct 2022 10:25:13 GMT  
		Size: 14.0 MB (14001566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334954d04c67d43f4bab0b7774053bae33c535a25cc073cf20528174bf6031e9`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:88717c434912a73202d619948c3352c352ada39682e290da1f669685783ea910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:8afe44a488e53c20b13d522ec0ceebf2f0574842e925f07709c4e3d0b34f95f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133500203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ef5b1bdbe7e51c149802adead793b95a3f4e9401df9c248dafef6e7294b9c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:16:54 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 21:18:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 21:18:32 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 21:18:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:18:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 21:18:32 GMT
WORKDIR /go
# Fri, 07 Oct 2022 04:35:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 04:35:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 04:35:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bccb3a1cff3b5f09bf1f21ba9ecb17c96329fb82f96605d922cfa4c9a82032`  
		Last Modified: Thu, 06 Oct 2022 21:25:08 GMT  
		Size: 122.3 MB (122251850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861cc3991b26fba6073631f27a1dc32bb27761195d912d05ee2f14b86fdf923f`  
		Last Modified: Thu, 06 Oct 2022 21:24:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f2801ecd75adee5f8c5111452c62dc9f74792e9de35771fdfaefcbe7a0004`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 6.9 MB (6941675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7494f25de5033fa48dcef9b9c880c76374b6d46092abb245fcd7ab1630c3bc`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 1.2 MB (1215177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8311897198e14fac14b1264d5fbc6cf8a02e580d706710353c401c0dcc67db`  
		Last Modified: Fri, 07 Oct 2022 04:35:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ceea5dfce2518bcd8f64951d0ff884bf4095037fb3ab84e81906b08889df2d4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8e6fb6b7549d30243de47d0ae0941d19a90e2f8240c24bdb7251033978fca3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:11:46 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:11:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:11:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:11:47 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:17:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:17:08 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:17:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:17:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:17:09 GMT
WORKDIR /go
# Sat, 08 Oct 2022 04:10:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 04:10:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 04:10:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 04:10:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b209b3d969f9a6352713d282fb4886bd906bc33154c9cc8af888e98292c36b82`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 284.7 KB (284689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3395a0d64b34009f33e3342948746a724fb68d28da16a8c474dcc6bd23b0c43`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f8b0abc05e00a9f055ae9fd2c0be61b1a031af3c0b983fde6989f6e51ad7e0`  
		Last Modified: Thu, 06 Oct 2022 20:33:21 GMT  
		Size: 118.6 MB (118635631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4ee43ba58df1ff51543e748374733cb56659f2f6cb2721e8bc55c9890bcd0`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f27e01fe424a71960c06a9bd9fdc198093ba0f8b341751f023e38129f1e52c`  
		Last Modified: Sat, 08 Oct 2022 04:11:06 GMT  
		Size: 6.8 MB (6808211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075d7a9278ef172ecaca28f1c74c6b1e45d8bfca5020998906df156bd9c93fdd`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 1.2 MB (1162977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f1f43b555f240d68b1d9f6fe17afdf4c78e8e165647d63558630489e43a713`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd54394bf4e39ecdbc7e7d3dc0ee1d3ec08689a5ad3f2a88563fe43a832d17e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab34ca7968e24f2883fb33f8c47da903cc3624ef5e9deb8e81fb8b51f537873`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:42:30 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:42:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 09:42:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:42:31 GMT
ENV GOLANG_VERSION=1.19.2
# Fri, 07 Oct 2022 09:49:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 07 Oct 2022 09:49:17 GMT
ENV GOPATH=/go
# Fri, 07 Oct 2022 09:49:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Oct 2022 09:49:18 GMT
WORKDIR /go
# Sat, 08 Oct 2022 05:06:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 05:06:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 05:06:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 05:06:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696b6cfba363e13486429ea964f92d832576e4e325397220afd2bff997ba045e`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 283.8 KB (283833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36573bb19dc804c15c8330b01de52ed6ded232a8b41d97998f1e33dee9f566a`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ebc5ada276c15274499e4bd347524b7eaaf42a3888a39db1464ecbaa94b9bf`  
		Last Modified: Fri, 07 Oct 2022 10:11:37 GMT  
		Size: 118.4 MB (118407461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5cc4edb1d1a08d0f82ac21910cc474b722bc371eaf97854b4bc90bc510ff00`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d7e71e64d4cde859c68147f4553124c90cf089314f225fdac27bb4729bc9c`  
		Last Modified: Sat, 08 Oct 2022 05:07:15 GMT  
		Size: 6.1 MB (6067873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf987d1eb410ed1530e75bbacb120d3efdc0437b5f68498cefae3d3245c4796`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800152f3498af5a4fbf7080d3044380f9826b5a1bf425001fa97d07ad544c736`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0ad855f7de2535a05dfc88f757a8ef1611a4578b85878ab2702e74994df4788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127986179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7396ddf3c1a000bdb6b5af6988bea71929050e5ea3c75b002f197fe6c6e25b9c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:48:18 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:48:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:48:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:48:21 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:49:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:49:56 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:49:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:49:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:49:59 GMT
WORKDIR /go
# Fri, 07 Oct 2022 08:01:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 08:01:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 08:01:29 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 08:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 08:01:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 08:01:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32db5db73116c723916b5df8f4ecc82d84f63f631c631d3fb81997d2fac11e9`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 284.5 KB (284532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c4b47475fc8104adcd7d897577b956078999e0cd332ec303fb21a18afcdf5c`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0598bfe6371f5c8223832079b9667d26a8bc5af5d1d818f5024e9c87d05a6`  
		Last Modified: Thu, 06 Oct 2022 20:57:08 GMT  
		Size: 116.8 MB (116820465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842c93ce66ef4b140121bbb9ec3badaa6b13b0f1a2a5a41e0bf5e4c8be8f852`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6608dc3160f80058977aa4f009e5ae9259e3278c7aa3ebf51ec2591c2090c`  
		Last Modified: Fri, 07 Oct 2022 08:02:20 GMT  
		Size: 7.1 MB (7052389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d63d110dcc7cc9d89ca5208169caa5cb389f3642ef114aead98e78606abc453`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3668944d647311a88fe8c1411dd9605faca9b1a213638d98ac647a5393f7adc6`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1750e31a6fb068abd57a4ca292cd0af0d488933c2286cc4fd3af92c7fd99702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128882306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e5ee9ab3729bc56e61c0311ee23fed2b88f72d89ead3e72ae4c1ce1369d99`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:26:03 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:28:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:28:54 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:28:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:28:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:28:56 GMT
WORKDIR /go
# Fri, 07 Oct 2022 07:56:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 07:56:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 07:56:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 07:56:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc648016b9956cdd58a13effd397263f1567720781730dc871f726e8cbf6dcb`  
		Last Modified: Thu, 06 Oct 2022 20:39:46 GMT  
		Size: 117.2 MB (117205225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c925b92d3e6aa9d43f83a9b3ea72790d539b1d983ddcffb8b95cf09a1e95e`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3131dd802f2ea71908bb86e0184679d69b9eccc01df8bd28eb998d3323d66063`  
		Last Modified: Fri, 07 Oct 2022 07:57:28 GMT  
		Size: 7.5 MB (7482443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82d9ca26c65fb5672a48eb58105343c6e06796084b0599b13f858bf22efbbd`  
		Last Modified: Fri, 07 Oct 2022 07:57:27 GMT  
		Size: 1.1 MB (1103855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396418b7a946c59b42806f6c5dcb72b12da6296dde780614b39c0733e2d5f6f`  
		Last Modified: Fri, 07 Oct 2022 07:57:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:4babe26aa4db963e2c1ba319a0f8e9a96c54a10c46dde7d0222f1889fe055d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131829172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e088de34239daf3a02ff2b831d410cbd9ef7c66fbeffc20a99f578027e437853`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:16:12 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:18:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:18:43 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:18:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:18:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:18:44 GMT
WORKDIR /go
# Fri, 07 Oct 2022 10:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 10:24:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 10:24:28 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 10:24:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 10:24:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 10:24:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3229342a30d3f1b9300228f7e3414e521024d8294398cc78d68c228dc8d1c40`  
		Last Modified: Thu, 06 Oct 2022 20:27:07 GMT  
		Size: 120.7 MB (120732457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e365613c053faa0517c5a9a3a8561d8dc4efe2d2d1159866dae02b07eb9f38d3`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca88f390fc5368bde96f7ab5aefec4cc5b192f7a443dc75ba03f35657b6ef4`  
		Last Modified: Fri, 07 Oct 2022 10:25:25 GMT  
		Size: 7.1 MB (7053036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2a2b0715c0c7b6eb7481142dfbc5e20109831c91458b10da2c70fb1c5a93fe`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 1.2 MB (1167415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad9784cee46592eb85a25958acb5461a20bdc2ce52e0d09405dcc330288022`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:fce8cf0a954111a1cb7e15ec8c9cf74dec576c92059e0a9cd3dadedffeee1cfb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888597946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67b82a73ab94a2525eb495091fbc693b28af993fc6cafbb3768c824f32acf18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:44:27 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:02 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:49:04 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:35:50 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:07 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c61bfb24309aadc8d001a8f706cedd3583ce2125fb7bc1628b7a83cfc7bb33`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e32dad104a4eff9e37934f63302fd3fa0226a9bdca330621819352ea66c94`  
		Last Modified: Tue, 04 Oct 2022 20:14:22 GMT  
		Size: 157.6 MB (157622445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f32605b45357608ad3962e2c0e0b6a16950c0958e61a5ea142b25f285bb21`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf8da2a2b79782e508e1f0cb603dc595be9caf18e69e6d38f5d00b4ddcc68f`  
		Last Modified: Tue, 04 Oct 2022 20:38:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724ca131e07cfb838c3f0fcfb2a103ce9b4f53dd0192aa29dcc63d376a10ba1`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d742c8bb37a68aed95adcd87d5288c1b3cd6f125cbe580316071c24e6dabd`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db91b0bb8cd4047b2e49a3be46d6ba19d1310228b61c3ad19969a9e2b0af5d6`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e44bf097cee24852462f4634e99e2f7620b77dc3842d687791c926c5a48de56`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.6 MB (1630878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bfff7b454e1e2bbc5b8cfff2ace2a606e33a84bb251fd6edc3e906e6addbe`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:ca9809a34b96a52e7e6eeef8d2057c1ba1a1a601eec7d91189d4b28e04573019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532828578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430f6ae7d3a4c215ba209863ecea0ab3685b63ad0aba36bf2b83eb90958b4ac8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:48:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:48:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:48:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:48:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:49:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:49:30 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:49:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:40:59 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:44:14 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:44:16 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:37:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:37:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:37:19 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:37:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6316baacdbe5997d732fa3555c0cd6f52fd467b41d4d41b596d460cfe8aa`  
		Last Modified: Wed, 14 Sep 2022 13:23:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de847c6f89452694f7278d29e3920062ee79faf74467742e329a71dc1db8805`  
		Last Modified: Wed, 14 Sep 2022 13:23:32 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1a6aca4358241a5ae1012bcd11240db54df9849aa25d07166c302dd3014dee`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0740ce986dad4039bc222ec6cfe798adfe4573d313d4e3583b8694109298e`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ed2e7f7ad8700539fdcbbfa0a73ce470c9b68aad955ee06135135e35f19d3`  
		Last Modified: Wed, 14 Sep 2022 13:23:39 GMT  
		Size: 25.7 MB (25676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde228a76aaef32add4bb50c16be55584a1328125aa2b2436d22da9d311837a4`  
		Last Modified: Wed, 14 Sep 2022 13:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab59b5ad3cb6d91ad9c3a3064155bffbd0cafff4fa66dc0d04e68d873a23c2c9`  
		Last Modified: Wed, 14 Sep 2022 13:23:29 GMT  
		Size: 526.6 KB (526562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7b60da979d12d87db1ff1c51bfbdabdf15744a9fc23c48d1f527d0d64a525`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915d3981a43f92982ff6e6db42d677c0a5c719a6956d8a7fc5fdcbf22a69837e`  
		Last Modified: Tue, 04 Oct 2022 20:13:30 GMT  
		Size: 157.8 MB (157822684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80571c0669f0277abd15b39422c7ac33098824b4e3acd5165a1094baff1c24a0`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce18cf0a5122414eb1417b6ea89e2af5dcbcfe8c8122f793c70530b5dfe185`  
		Last Modified: Tue, 04 Oct 2022 20:38:56 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6550656e761fb3dd33274b46efce609cf133d7ed5c3d2225307cb86e915686`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa241376abdf364b18ef913f22cd27f760430d56204f746263e788237ad2bc7b`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b0bbe614d6c4745bef5fb8c12ed68f7b5098aba644c3702b2c751772ff8dca`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83010d61e0e222aba800d09aa0e6f101273aa57850a02045c234cf45a46c26a`  
		Last Modified: Tue, 04 Oct 2022 20:38:54 GMT  
		Size: 1.8 MB (1834812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cece43f8685aa24f6224e5c09637d5766d50638f619e13f1ea4f6f5a6797992`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:22a859f3d66929d869a26302a0acd2b8e2bcfb183a16037de3cb3a0b142bfae6
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
$ docker pull caddy@sha256:8afe44a488e53c20b13d522ec0ceebf2f0574842e925f07709c4e3d0b34f95f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133500203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ef5b1bdbe7e51c149802adead793b95a3f4e9401df9c248dafef6e7294b9c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:16:54 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 21:18:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 21:18:32 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 21:18:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:18:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 21:18:32 GMT
WORKDIR /go
# Fri, 07 Oct 2022 04:35:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 04:35:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 04:35:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bccb3a1cff3b5f09bf1f21ba9ecb17c96329fb82f96605d922cfa4c9a82032`  
		Last Modified: Thu, 06 Oct 2022 21:25:08 GMT  
		Size: 122.3 MB (122251850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861cc3991b26fba6073631f27a1dc32bb27761195d912d05ee2f14b86fdf923f`  
		Last Modified: Thu, 06 Oct 2022 21:24:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f2801ecd75adee5f8c5111452c62dc9f74792e9de35771fdfaefcbe7a0004`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 6.9 MB (6941675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7494f25de5033fa48dcef9b9c880c76374b6d46092abb245fcd7ab1630c3bc`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 1.2 MB (1215177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8311897198e14fac14b1264d5fbc6cf8a02e580d706710353c401c0dcc67db`  
		Last Modified: Fri, 07 Oct 2022 04:35:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ceea5dfce2518bcd8f64951d0ff884bf4095037fb3ab84e81906b08889df2d4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8e6fb6b7549d30243de47d0ae0941d19a90e2f8240c24bdb7251033978fca3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:11:46 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:11:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:11:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:11:47 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:17:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:17:08 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:17:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:17:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:17:09 GMT
WORKDIR /go
# Sat, 08 Oct 2022 04:10:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 04:10:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 04:10:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 04:10:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b209b3d969f9a6352713d282fb4886bd906bc33154c9cc8af888e98292c36b82`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 284.7 KB (284689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3395a0d64b34009f33e3342948746a724fb68d28da16a8c474dcc6bd23b0c43`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f8b0abc05e00a9f055ae9fd2c0be61b1a031af3c0b983fde6989f6e51ad7e0`  
		Last Modified: Thu, 06 Oct 2022 20:33:21 GMT  
		Size: 118.6 MB (118635631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4ee43ba58df1ff51543e748374733cb56659f2f6cb2721e8bc55c9890bcd0`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f27e01fe424a71960c06a9bd9fdc198093ba0f8b341751f023e38129f1e52c`  
		Last Modified: Sat, 08 Oct 2022 04:11:06 GMT  
		Size: 6.8 MB (6808211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075d7a9278ef172ecaca28f1c74c6b1e45d8bfca5020998906df156bd9c93fdd`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 1.2 MB (1162977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f1f43b555f240d68b1d9f6fe17afdf4c78e8e165647d63558630489e43a713`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd54394bf4e39ecdbc7e7d3dc0ee1d3ec08689a5ad3f2a88563fe43a832d17e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab34ca7968e24f2883fb33f8c47da903cc3624ef5e9deb8e81fb8b51f537873`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:42:30 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:42:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 09:42:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:42:31 GMT
ENV GOLANG_VERSION=1.19.2
# Fri, 07 Oct 2022 09:49:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 07 Oct 2022 09:49:17 GMT
ENV GOPATH=/go
# Fri, 07 Oct 2022 09:49:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Oct 2022 09:49:18 GMT
WORKDIR /go
# Sat, 08 Oct 2022 05:06:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 05:06:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 05:06:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 05:06:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696b6cfba363e13486429ea964f92d832576e4e325397220afd2bff997ba045e`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 283.8 KB (283833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36573bb19dc804c15c8330b01de52ed6ded232a8b41d97998f1e33dee9f566a`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ebc5ada276c15274499e4bd347524b7eaaf42a3888a39db1464ecbaa94b9bf`  
		Last Modified: Fri, 07 Oct 2022 10:11:37 GMT  
		Size: 118.4 MB (118407461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5cc4edb1d1a08d0f82ac21910cc474b722bc371eaf97854b4bc90bc510ff00`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d7e71e64d4cde859c68147f4553124c90cf089314f225fdac27bb4729bc9c`  
		Last Modified: Sat, 08 Oct 2022 05:07:15 GMT  
		Size: 6.1 MB (6067873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf987d1eb410ed1530e75bbacb120d3efdc0437b5f68498cefae3d3245c4796`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800152f3498af5a4fbf7080d3044380f9826b5a1bf425001fa97d07ad544c736`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0ad855f7de2535a05dfc88f757a8ef1611a4578b85878ab2702e74994df4788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127986179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7396ddf3c1a000bdb6b5af6988bea71929050e5ea3c75b002f197fe6c6e25b9c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:48:18 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:48:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:48:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:48:21 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:49:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:49:56 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:49:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:49:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:49:59 GMT
WORKDIR /go
# Fri, 07 Oct 2022 08:01:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 08:01:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 08:01:29 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 08:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 08:01:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 08:01:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32db5db73116c723916b5df8f4ecc82d84f63f631c631d3fb81997d2fac11e9`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 284.5 KB (284532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c4b47475fc8104adcd7d897577b956078999e0cd332ec303fb21a18afcdf5c`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0598bfe6371f5c8223832079b9667d26a8bc5af5d1d818f5024e9c87d05a6`  
		Last Modified: Thu, 06 Oct 2022 20:57:08 GMT  
		Size: 116.8 MB (116820465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842c93ce66ef4b140121bbb9ec3badaa6b13b0f1a2a5a41e0bf5e4c8be8f852`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6608dc3160f80058977aa4f009e5ae9259e3278c7aa3ebf51ec2591c2090c`  
		Last Modified: Fri, 07 Oct 2022 08:02:20 GMT  
		Size: 7.1 MB (7052389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d63d110dcc7cc9d89ca5208169caa5cb389f3642ef114aead98e78606abc453`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3668944d647311a88fe8c1411dd9605faca9b1a213638d98ac647a5393f7adc6`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1750e31a6fb068abd57a4ca292cd0af0d488933c2286cc4fd3af92c7fd99702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128882306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e5ee9ab3729bc56e61c0311ee23fed2b88f72d89ead3e72ae4c1ce1369d99`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:26:03 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:28:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:28:54 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:28:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:28:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:28:56 GMT
WORKDIR /go
# Fri, 07 Oct 2022 07:56:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 07:56:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 07:56:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 07:56:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc648016b9956cdd58a13effd397263f1567720781730dc871f726e8cbf6dcb`  
		Last Modified: Thu, 06 Oct 2022 20:39:46 GMT  
		Size: 117.2 MB (117205225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c925b92d3e6aa9d43f83a9b3ea72790d539b1d983ddcffb8b95cf09a1e95e`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3131dd802f2ea71908bb86e0184679d69b9eccc01df8bd28eb998d3323d66063`  
		Last Modified: Fri, 07 Oct 2022 07:57:28 GMT  
		Size: 7.5 MB (7482443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82d9ca26c65fb5672a48eb58105343c6e06796084b0599b13f858bf22efbbd`  
		Last Modified: Fri, 07 Oct 2022 07:57:27 GMT  
		Size: 1.1 MB (1103855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396418b7a946c59b42806f6c5dcb72b12da6296dde780614b39c0733e2d5f6f`  
		Last Modified: Fri, 07 Oct 2022 07:57:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4babe26aa4db963e2c1ba319a0f8e9a96c54a10c46dde7d0222f1889fe055d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131829172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e088de34239daf3a02ff2b831d410cbd9ef7c66fbeffc20a99f578027e437853`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:16:12 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:18:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:18:43 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:18:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:18:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:18:44 GMT
WORKDIR /go
# Fri, 07 Oct 2022 10:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 10:24:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 10:24:28 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 10:24:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 10:24:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 10:24:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3229342a30d3f1b9300228f7e3414e521024d8294398cc78d68c228dc8d1c40`  
		Last Modified: Thu, 06 Oct 2022 20:27:07 GMT  
		Size: 120.7 MB (120732457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e365613c053faa0517c5a9a3a8561d8dc4efe2d2d1159866dae02b07eb9f38d3`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca88f390fc5368bde96f7ab5aefec4cc5b192f7a443dc75ba03f35657b6ef4`  
		Last Modified: Fri, 07 Oct 2022 10:25:25 GMT  
		Size: 7.1 MB (7053036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2a2b0715c0c7b6eb7481142dfbc5e20109831c91458b10da2c70fb1c5a93fe`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 1.2 MB (1167415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad9784cee46592eb85a25958acb5461a20bdc2ce52e0d09405dcc330288022`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f6c3f33dda0aad41a0d698c876064a5aca204d85fb603e864d89b065f92014cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:fce8cf0a954111a1cb7e15ec8c9cf74dec576c92059e0a9cd3dadedffeee1cfb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888597946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67b82a73ab94a2525eb495091fbc693b28af993fc6cafbb3768c824f32acf18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:44:27 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:02 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:49:04 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:35:50 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:07 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c61bfb24309aadc8d001a8f706cedd3583ce2125fb7bc1628b7a83cfc7bb33`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e32dad104a4eff9e37934f63302fd3fa0226a9bdca330621819352ea66c94`  
		Last Modified: Tue, 04 Oct 2022 20:14:22 GMT  
		Size: 157.6 MB (157622445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f32605b45357608ad3962e2c0e0b6a16950c0958e61a5ea142b25f285bb21`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf8da2a2b79782e508e1f0cb603dc595be9caf18e69e6d38f5d00b4ddcc68f`  
		Last Modified: Tue, 04 Oct 2022 20:38:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724ca131e07cfb838c3f0fcfb2a103ce9b4f53dd0192aa29dcc63d376a10ba1`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d742c8bb37a68aed95adcd87d5288c1b3cd6f125cbe580316071c24e6dabd`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db91b0bb8cd4047b2e49a3be46d6ba19d1310228b61c3ad19969a9e2b0af5d6`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e44bf097cee24852462f4634e99e2f7620b77dc3842d687791c926c5a48de56`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.6 MB (1630878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bfff7b454e1e2bbc5b8cfff2ace2a606e33a84bb251fd6edc3e906e6addbe`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:482053b6811d642bb974423087fbf568468ffc9cf170dac246d1ff6779177eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:ca9809a34b96a52e7e6eeef8d2057c1ba1a1a601eec7d91189d4b28e04573019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532828578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430f6ae7d3a4c215ba209863ecea0ab3685b63ad0aba36bf2b83eb90958b4ac8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:48:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:48:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:48:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:48:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:49:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:49:30 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:49:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:40:59 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:44:14 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:44:16 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:37:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:37:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:37:19 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:37:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6316baacdbe5997d732fa3555c0cd6f52fd467b41d4d41b596d460cfe8aa`  
		Last Modified: Wed, 14 Sep 2022 13:23:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de847c6f89452694f7278d29e3920062ee79faf74467742e329a71dc1db8805`  
		Last Modified: Wed, 14 Sep 2022 13:23:32 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1a6aca4358241a5ae1012bcd11240db54df9849aa25d07166c302dd3014dee`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0740ce986dad4039bc222ec6cfe798adfe4573d313d4e3583b8694109298e`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ed2e7f7ad8700539fdcbbfa0a73ce470c9b68aad955ee06135135e35f19d3`  
		Last Modified: Wed, 14 Sep 2022 13:23:39 GMT  
		Size: 25.7 MB (25676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde228a76aaef32add4bb50c16be55584a1328125aa2b2436d22da9d311837a4`  
		Last Modified: Wed, 14 Sep 2022 13:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab59b5ad3cb6d91ad9c3a3064155bffbd0cafff4fa66dc0d04e68d873a23c2c9`  
		Last Modified: Wed, 14 Sep 2022 13:23:29 GMT  
		Size: 526.6 KB (526562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7b60da979d12d87db1ff1c51bfbdabdf15744a9fc23c48d1f527d0d64a525`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915d3981a43f92982ff6e6db42d677c0a5c719a6956d8a7fc5fdcbf22a69837e`  
		Last Modified: Tue, 04 Oct 2022 20:13:30 GMT  
		Size: 157.8 MB (157822684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80571c0669f0277abd15b39422c7ac33098824b4e3acd5165a1094baff1c24a0`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce18cf0a5122414eb1417b6ea89e2af5dcbcfe8c8122f793c70530b5dfe185`  
		Last Modified: Tue, 04 Oct 2022 20:38:56 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6550656e761fb3dd33274b46efce609cf133d7ed5c3d2225307cb86e915686`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa241376abdf364b18ef913f22cd27f760430d56204f746263e788237ad2bc7b`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b0bbe614d6c4745bef5fb8c12ed68f7b5098aba644c3702b2c751772ff8dca`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83010d61e0e222aba800d09aa0e6f101273aa57850a02045c234cf45a46c26a`  
		Last Modified: Tue, 04 Oct 2022 20:38:54 GMT  
		Size: 1.8 MB (1834812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cece43f8685aa24f6224e5c09637d5766d50638f619e13f1ea4f6f5a6797992`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:a2f4650d657ce94148fda7db712cc27b1cf037cd53535cdcfe6021488cb35680
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f65a2a6e954346897215a9d2fa42d57afe06720d80aa6f5ee846aea9dd2343e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:391c3e9d6a79f66b9cfdc3800ac89da113665ef28bd627bc2ae077a8fdffa0d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1`

```console
$ docker pull caddy@sha256:3f766f2dc97b6440bb6dcc8f105279999c60d6e0382403d7ab3be51329a692cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:2.6.1` - linux; amd64

```console
$ docker pull caddy@sha256:5e68e231a2fb583cc2bafe472844495cd9c1b119b626cb61777a75f990886906
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181f13e1cc5fd90d0b4869e57689b5200589ca1029971fc7233082c04806a55b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 04:34:57 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:34:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 04:34:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 04:35:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 04:35:01 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 04:35:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890b94b17a6b1f257ddec10a103ff342db99516b0d339260623d6610db9b1349`  
		Last Modified: Fri, 07 Oct 2022 04:35:27 GMT  
		Size: 14.5 MB (14493818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d852ea4bd9f60570e83e432bcb361e0400dc3b2c3a264a447dfc2f6b292c0a`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:12eface0625a91f60ec1e6f8ccd864d52c9dc69f3b02ea126e4fdaacf8de5bd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0d4211357adf7a3124613f982947e3745803a9205db56b524ae70f1f03f521`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 04:09:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 08 Oct 2022 04:09:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Sat, 08 Oct 2022 04:09:55 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:09:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 08 Oct 2022 04:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 80
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443/udp
# Sat, 08 Oct 2022 04:10:00 GMT
EXPOSE 2019
# Sat, 08 Oct 2022 04:10:00 GMT
WORKDIR /srv
# Sat, 08 Oct 2022 04:10:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa0e79d89709c451dcc1ed2799b94c19204fb58ea7cce7895eef1f51c01bb50`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 304.5 KB (304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9215626c7fc1bfbffb15114b3a5de7fc64de1e7a2a21ee2056121f5ef65b2338`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ca8b546a2bb8c3467ac3eafdca5479dd6396e518b348315a1b16a18519b61`  
		Last Modified: Sat, 08 Oct 2022 04:10:49 GMT  
		Size: 13.8 MB (13848654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e20fa1676a89097bb7bfd9deb83ec1b2ba35972a2c365e7e0b111bf46a430`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8c5c01339078f89f85a5a7cd08d8bd89962900d295af83cc0eb70de31c4d51ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c275d9a5ca87dde16a12a6d524b9a542b9e77e96ead14f8c577857b6091f24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:17:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:17:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:17:46 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:17:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:17:52 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:17:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11d99bb68cba432782c86e461f4c830d8bc08ba0b2df2999db3ab67a55f57e`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 303.6 KB (303619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30dd3a0b20a2d25c12f53bf9ae92037f177e924b7613dbbeedca0029d44215`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0645b8aab72e227505345e7745508a1f23ed2ff304884458f31d828eac843`  
		Last Modified: Fri, 07 Oct 2022 07:18:46 GMT  
		Size: 13.8 MB (13824551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978d7d8e43141c7a175739d7aafcb64b5b8f6561efb3295d91c186bfab20eb3`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e6d1ad533fd36cd36a387471e708740876c809760795f8868490beab7d98443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1814d3a7f6c971e84b565c46272fc51961c9e67e0e8787781be733c087a22`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 08:00:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 08:00:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 08:00:59 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 08:01:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 08:01:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 08:01:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 08:01:06 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 08:01:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 08:01:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 08:01:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 08:01:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 08:01:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 08:01:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 08:01:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 08:01:14 GMT
EXPOSE 80
# Fri, 07 Oct 2022 08:01:15 GMT
EXPOSE 443
# Fri, 07 Oct 2022 08:01:16 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 08:01:17 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 08:01:18 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 08:01:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6fca9d7511cb60edf3b5df387d6b1fd5aaac17867575fc733cf40137b95a90`  
		Last Modified: Fri, 07 Oct 2022 08:02:04 GMT  
		Size: 304.3 KB (304303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8483ebae1fd52b4e5a413ddd322fedfc3978bd5f95dfd62ea2c53f1a0b7a7e05`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ad12dc08ecd5447289e06895740be336d526d7bec274b5cab707b3be6c4df`  
		Last Modified: Fri, 07 Oct 2022 08:02:05 GMT  
		Size: 13.2 MB (13196260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b783a84a1d985b8c4d150880a665dffed5e8d3cd282ed0f45af0b28e45c30a`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:3c296624df3a6ffb31e3a5eca10b509c80150fe12e9b19ebf27e061189d44278
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4250b6ab2344a47d567b072f8080c8f6aa93b04bd773b51fa57148ac08e30379`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:56:13 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:56:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:56:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:56:22 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:56:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d070e557e928b65136b4bb037dd73ddfb5be784310db1f0f3640ce1216afc`  
		Last Modified: Fri, 07 Oct 2022 07:57:11 GMT  
		Size: 12.9 MB (12853693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40adebe65a7cbe002c94177299a2ae8a216f554d7d6ae5eec0916ba7330da421`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; s390x

```console
$ docker pull caddy@sha256:3e5aa9861d4d5e9c0dfda105fa0b598ee20d5f254b734f5a418c99f6a5b9b5af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2a3441daa59cefaa1dbb6d0edd094f53abe4b3c89877fd3b7121dd53d15ef3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 10:23:51 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:23:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 10:24:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 10:24:04 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 10:24:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 10:24:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 10:24:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 10:24:09 GMT
EXPOSE 80
# Fri, 07 Oct 2022 10:24:10 GMT
EXPOSE 443
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 10:24:12 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 10:24:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8c37b8106cb4218c6396b95deabef48406b60274cd3304a53e50b645cd9e7`  
		Last Modified: Fri, 07 Oct 2022 10:25:13 GMT  
		Size: 14.0 MB (14001566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334954d04c67d43f4bab0b7774053bae33c535a25cc073cf20528174bf6031e9`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-alpine`

```console
$ docker pull caddy@sha256:75d2e29d0c3ec9aa78e640c022d5afec48c2c8ccefe0f956280f66bcced7cceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:5e68e231a2fb583cc2bafe472844495cd9c1b119b626cb61777a75f990886906
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181f13e1cc5fd90d0b4869e57689b5200589ca1029971fc7233082c04806a55b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 04:34:57 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:34:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 04:34:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 04:35:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 04:35:01 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 04:35:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890b94b17a6b1f257ddec10a103ff342db99516b0d339260623d6610db9b1349`  
		Last Modified: Fri, 07 Oct 2022 04:35:27 GMT  
		Size: 14.5 MB (14493818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d852ea4bd9f60570e83e432bcb361e0400dc3b2c3a264a447dfc2f6b292c0a`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:12eface0625a91f60ec1e6f8ccd864d52c9dc69f3b02ea126e4fdaacf8de5bd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0d4211357adf7a3124613f982947e3745803a9205db56b524ae70f1f03f521`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 04:09:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 08 Oct 2022 04:09:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Sat, 08 Oct 2022 04:09:55 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:09:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 08 Oct 2022 04:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 80
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443/udp
# Sat, 08 Oct 2022 04:10:00 GMT
EXPOSE 2019
# Sat, 08 Oct 2022 04:10:00 GMT
WORKDIR /srv
# Sat, 08 Oct 2022 04:10:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa0e79d89709c451dcc1ed2799b94c19204fb58ea7cce7895eef1f51c01bb50`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 304.5 KB (304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9215626c7fc1bfbffb15114b3a5de7fc64de1e7a2a21ee2056121f5ef65b2338`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ca8b546a2bb8c3467ac3eafdca5479dd6396e518b348315a1b16a18519b61`  
		Last Modified: Sat, 08 Oct 2022 04:10:49 GMT  
		Size: 13.8 MB (13848654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e20fa1676a89097bb7bfd9deb83ec1b2ba35972a2c365e7e0b111bf46a430`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8c5c01339078f89f85a5a7cd08d8bd89962900d295af83cc0eb70de31c4d51ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c275d9a5ca87dde16a12a6d524b9a542b9e77e96ead14f8c577857b6091f24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:17:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:17:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:17:46 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:17:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:17:52 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:17:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11d99bb68cba432782c86e461f4c830d8bc08ba0b2df2999db3ab67a55f57e`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 303.6 KB (303619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30dd3a0b20a2d25c12f53bf9ae92037f177e924b7613dbbeedca0029d44215`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0645b8aab72e227505345e7745508a1f23ed2ff304884458f31d828eac843`  
		Last Modified: Fri, 07 Oct 2022 07:18:46 GMT  
		Size: 13.8 MB (13824551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978d7d8e43141c7a175739d7aafcb64b5b8f6561efb3295d91c186bfab20eb3`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e6d1ad533fd36cd36a387471e708740876c809760795f8868490beab7d98443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1814d3a7f6c971e84b565c46272fc51961c9e67e0e8787781be733c087a22`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 08:00:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 08:00:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 08:00:59 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 08:01:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 08:01:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 08:01:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 08:01:06 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 08:01:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 08:01:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 08:01:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 08:01:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 08:01:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 08:01:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 08:01:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 08:01:14 GMT
EXPOSE 80
# Fri, 07 Oct 2022 08:01:15 GMT
EXPOSE 443
# Fri, 07 Oct 2022 08:01:16 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 08:01:17 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 08:01:18 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 08:01:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6fca9d7511cb60edf3b5df387d6b1fd5aaac17867575fc733cf40137b95a90`  
		Last Modified: Fri, 07 Oct 2022 08:02:04 GMT  
		Size: 304.3 KB (304303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8483ebae1fd52b4e5a413ddd322fedfc3978bd5f95dfd62ea2c53f1a0b7a7e05`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ad12dc08ecd5447289e06895740be336d526d7bec274b5cab707b3be6c4df`  
		Last Modified: Fri, 07 Oct 2022 08:02:05 GMT  
		Size: 13.2 MB (13196260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b783a84a1d985b8c4d150880a665dffed5e8d3cd282ed0f45af0b28e45c30a`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:3c296624df3a6ffb31e3a5eca10b509c80150fe12e9b19ebf27e061189d44278
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4250b6ab2344a47d567b072f8080c8f6aa93b04bd773b51fa57148ac08e30379`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:56:13 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:56:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:56:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:56:22 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:56:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d070e557e928b65136b4bb037dd73ddfb5be784310db1f0f3640ce1216afc`  
		Last Modified: Fri, 07 Oct 2022 07:57:11 GMT  
		Size: 12.9 MB (12853693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40adebe65a7cbe002c94177299a2ae8a216f554d7d6ae5eec0916ba7330da421`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3e5aa9861d4d5e9c0dfda105fa0b598ee20d5f254b734f5a418c99f6a5b9b5af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2a3441daa59cefaa1dbb6d0edd094f53abe4b3c89877fd3b7121dd53d15ef3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 10:23:51 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:23:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 10:24:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 10:24:04 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 10:24:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 10:24:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 10:24:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 10:24:09 GMT
EXPOSE 80
# Fri, 07 Oct 2022 10:24:10 GMT
EXPOSE 443
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 10:24:12 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 10:24:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8c37b8106cb4218c6396b95deabef48406b60274cd3304a53e50b645cd9e7`  
		Last Modified: Fri, 07 Oct 2022 10:25:13 GMT  
		Size: 14.0 MB (14001566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334954d04c67d43f4bab0b7774053bae33c535a25cc073cf20528174bf6031e9`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-builder`

```console
$ docker pull caddy@sha256:88717c434912a73202d619948c3352c352ada39682e290da1f669685783ea910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:2.6.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:8afe44a488e53c20b13d522ec0ceebf2f0574842e925f07709c4e3d0b34f95f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133500203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ef5b1bdbe7e51c149802adead793b95a3f4e9401df9c248dafef6e7294b9c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:16:54 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 21:18:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 21:18:32 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 21:18:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:18:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 21:18:32 GMT
WORKDIR /go
# Fri, 07 Oct 2022 04:35:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 04:35:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 04:35:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bccb3a1cff3b5f09bf1f21ba9ecb17c96329fb82f96605d922cfa4c9a82032`  
		Last Modified: Thu, 06 Oct 2022 21:25:08 GMT  
		Size: 122.3 MB (122251850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861cc3991b26fba6073631f27a1dc32bb27761195d912d05ee2f14b86fdf923f`  
		Last Modified: Thu, 06 Oct 2022 21:24:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f2801ecd75adee5f8c5111452c62dc9f74792e9de35771fdfaefcbe7a0004`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 6.9 MB (6941675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7494f25de5033fa48dcef9b9c880c76374b6d46092abb245fcd7ab1630c3bc`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 1.2 MB (1215177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8311897198e14fac14b1264d5fbc6cf8a02e580d706710353c401c0dcc67db`  
		Last Modified: Fri, 07 Oct 2022 04:35:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ceea5dfce2518bcd8f64951d0ff884bf4095037fb3ab84e81906b08889df2d4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8e6fb6b7549d30243de47d0ae0941d19a90e2f8240c24bdb7251033978fca3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:11:46 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:11:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:11:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:11:47 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:17:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:17:08 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:17:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:17:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:17:09 GMT
WORKDIR /go
# Sat, 08 Oct 2022 04:10:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 04:10:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 04:10:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 04:10:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b209b3d969f9a6352713d282fb4886bd906bc33154c9cc8af888e98292c36b82`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 284.7 KB (284689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3395a0d64b34009f33e3342948746a724fb68d28da16a8c474dcc6bd23b0c43`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f8b0abc05e00a9f055ae9fd2c0be61b1a031af3c0b983fde6989f6e51ad7e0`  
		Last Modified: Thu, 06 Oct 2022 20:33:21 GMT  
		Size: 118.6 MB (118635631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4ee43ba58df1ff51543e748374733cb56659f2f6cb2721e8bc55c9890bcd0`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f27e01fe424a71960c06a9bd9fdc198093ba0f8b341751f023e38129f1e52c`  
		Last Modified: Sat, 08 Oct 2022 04:11:06 GMT  
		Size: 6.8 MB (6808211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075d7a9278ef172ecaca28f1c74c6b1e45d8bfca5020998906df156bd9c93fdd`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 1.2 MB (1162977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f1f43b555f240d68b1d9f6fe17afdf4c78e8e165647d63558630489e43a713`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd54394bf4e39ecdbc7e7d3dc0ee1d3ec08689a5ad3f2a88563fe43a832d17e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab34ca7968e24f2883fb33f8c47da903cc3624ef5e9deb8e81fb8b51f537873`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:42:30 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:42:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 09:42:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:42:31 GMT
ENV GOLANG_VERSION=1.19.2
# Fri, 07 Oct 2022 09:49:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 07 Oct 2022 09:49:17 GMT
ENV GOPATH=/go
# Fri, 07 Oct 2022 09:49:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Oct 2022 09:49:18 GMT
WORKDIR /go
# Sat, 08 Oct 2022 05:06:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 05:06:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 05:06:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 05:06:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696b6cfba363e13486429ea964f92d832576e4e325397220afd2bff997ba045e`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 283.8 KB (283833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36573bb19dc804c15c8330b01de52ed6ded232a8b41d97998f1e33dee9f566a`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ebc5ada276c15274499e4bd347524b7eaaf42a3888a39db1464ecbaa94b9bf`  
		Last Modified: Fri, 07 Oct 2022 10:11:37 GMT  
		Size: 118.4 MB (118407461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5cc4edb1d1a08d0f82ac21910cc474b722bc371eaf97854b4bc90bc510ff00`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d7e71e64d4cde859c68147f4553124c90cf089314f225fdac27bb4729bc9c`  
		Last Modified: Sat, 08 Oct 2022 05:07:15 GMT  
		Size: 6.1 MB (6067873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf987d1eb410ed1530e75bbacb120d3efdc0437b5f68498cefae3d3245c4796`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800152f3498af5a4fbf7080d3044380f9826b5a1bf425001fa97d07ad544c736`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0ad855f7de2535a05dfc88f757a8ef1611a4578b85878ab2702e74994df4788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127986179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7396ddf3c1a000bdb6b5af6988bea71929050e5ea3c75b002f197fe6c6e25b9c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:48:18 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:48:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:48:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:48:21 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:49:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:49:56 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:49:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:49:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:49:59 GMT
WORKDIR /go
# Fri, 07 Oct 2022 08:01:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 08:01:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 08:01:29 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 08:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 08:01:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 08:01:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32db5db73116c723916b5df8f4ecc82d84f63f631c631d3fb81997d2fac11e9`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 284.5 KB (284532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c4b47475fc8104adcd7d897577b956078999e0cd332ec303fb21a18afcdf5c`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0598bfe6371f5c8223832079b9667d26a8bc5af5d1d818f5024e9c87d05a6`  
		Last Modified: Thu, 06 Oct 2022 20:57:08 GMT  
		Size: 116.8 MB (116820465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842c93ce66ef4b140121bbb9ec3badaa6b13b0f1a2a5a41e0bf5e4c8be8f852`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6608dc3160f80058977aa4f009e5ae9259e3278c7aa3ebf51ec2591c2090c`  
		Last Modified: Fri, 07 Oct 2022 08:02:20 GMT  
		Size: 7.1 MB (7052389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d63d110dcc7cc9d89ca5208169caa5cb389f3642ef114aead98e78606abc453`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3668944d647311a88fe8c1411dd9605faca9b1a213638d98ac647a5393f7adc6`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1750e31a6fb068abd57a4ca292cd0af0d488933c2286cc4fd3af92c7fd99702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128882306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e5ee9ab3729bc56e61c0311ee23fed2b88f72d89ead3e72ae4c1ce1369d99`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:26:03 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:28:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:28:54 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:28:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:28:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:28:56 GMT
WORKDIR /go
# Fri, 07 Oct 2022 07:56:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 07:56:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 07:56:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 07:56:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc648016b9956cdd58a13effd397263f1567720781730dc871f726e8cbf6dcb`  
		Last Modified: Thu, 06 Oct 2022 20:39:46 GMT  
		Size: 117.2 MB (117205225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c925b92d3e6aa9d43f83a9b3ea72790d539b1d983ddcffb8b95cf09a1e95e`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3131dd802f2ea71908bb86e0184679d69b9eccc01df8bd28eb998d3323d66063`  
		Last Modified: Fri, 07 Oct 2022 07:57:28 GMT  
		Size: 7.5 MB (7482443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82d9ca26c65fb5672a48eb58105343c6e06796084b0599b13f858bf22efbbd`  
		Last Modified: Fri, 07 Oct 2022 07:57:27 GMT  
		Size: 1.1 MB (1103855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396418b7a946c59b42806f6c5dcb72b12da6296dde780614b39c0733e2d5f6f`  
		Last Modified: Fri, 07 Oct 2022 07:57:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:4babe26aa4db963e2c1ba319a0f8e9a96c54a10c46dde7d0222f1889fe055d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131829172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e088de34239daf3a02ff2b831d410cbd9ef7c66fbeffc20a99f578027e437853`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:16:12 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:18:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:18:43 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:18:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:18:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:18:44 GMT
WORKDIR /go
# Fri, 07 Oct 2022 10:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 10:24:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 10:24:28 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 10:24:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 10:24:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 10:24:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3229342a30d3f1b9300228f7e3414e521024d8294398cc78d68c228dc8d1c40`  
		Last Modified: Thu, 06 Oct 2022 20:27:07 GMT  
		Size: 120.7 MB (120732457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e365613c053faa0517c5a9a3a8561d8dc4efe2d2d1159866dae02b07eb9f38d3`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca88f390fc5368bde96f7ab5aefec4cc5b192f7a443dc75ba03f35657b6ef4`  
		Last Modified: Fri, 07 Oct 2022 10:25:25 GMT  
		Size: 7.1 MB (7053036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2a2b0715c0c7b6eb7481142dfbc5e20109831c91458b10da2c70fb1c5a93fe`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 1.2 MB (1167415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad9784cee46592eb85a25958acb5461a20bdc2ce52e0d09405dcc330288022`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:fce8cf0a954111a1cb7e15ec8c9cf74dec576c92059e0a9cd3dadedffeee1cfb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888597946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67b82a73ab94a2525eb495091fbc693b28af993fc6cafbb3768c824f32acf18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:44:27 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:02 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:49:04 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:35:50 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:07 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c61bfb24309aadc8d001a8f706cedd3583ce2125fb7bc1628b7a83cfc7bb33`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e32dad104a4eff9e37934f63302fd3fa0226a9bdca330621819352ea66c94`  
		Last Modified: Tue, 04 Oct 2022 20:14:22 GMT  
		Size: 157.6 MB (157622445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f32605b45357608ad3962e2c0e0b6a16950c0958e61a5ea142b25f285bb21`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf8da2a2b79782e508e1f0cb603dc595be9caf18e69e6d38f5d00b4ddcc68f`  
		Last Modified: Tue, 04 Oct 2022 20:38:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724ca131e07cfb838c3f0fcfb2a103ce9b4f53dd0192aa29dcc63d376a10ba1`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d742c8bb37a68aed95adcd87d5288c1b3cd6f125cbe580316071c24e6dabd`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db91b0bb8cd4047b2e49a3be46d6ba19d1310228b61c3ad19969a9e2b0af5d6`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e44bf097cee24852462f4634e99e2f7620b77dc3842d687791c926c5a48de56`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.6 MB (1630878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bfff7b454e1e2bbc5b8cfff2ace2a606e33a84bb251fd6edc3e906e6addbe`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:ca9809a34b96a52e7e6eeef8d2057c1ba1a1a601eec7d91189d4b28e04573019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532828578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430f6ae7d3a4c215ba209863ecea0ab3685b63ad0aba36bf2b83eb90958b4ac8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:48:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:48:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:48:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:48:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:49:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:49:30 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:49:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:40:59 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:44:14 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:44:16 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:37:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:37:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:37:19 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:37:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6316baacdbe5997d732fa3555c0cd6f52fd467b41d4d41b596d460cfe8aa`  
		Last Modified: Wed, 14 Sep 2022 13:23:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de847c6f89452694f7278d29e3920062ee79faf74467742e329a71dc1db8805`  
		Last Modified: Wed, 14 Sep 2022 13:23:32 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1a6aca4358241a5ae1012bcd11240db54df9849aa25d07166c302dd3014dee`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0740ce986dad4039bc222ec6cfe798adfe4573d313d4e3583b8694109298e`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ed2e7f7ad8700539fdcbbfa0a73ce470c9b68aad955ee06135135e35f19d3`  
		Last Modified: Wed, 14 Sep 2022 13:23:39 GMT  
		Size: 25.7 MB (25676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde228a76aaef32add4bb50c16be55584a1328125aa2b2436d22da9d311837a4`  
		Last Modified: Wed, 14 Sep 2022 13:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab59b5ad3cb6d91ad9c3a3064155bffbd0cafff4fa66dc0d04e68d873a23c2c9`  
		Last Modified: Wed, 14 Sep 2022 13:23:29 GMT  
		Size: 526.6 KB (526562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7b60da979d12d87db1ff1c51bfbdabdf15744a9fc23c48d1f527d0d64a525`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915d3981a43f92982ff6e6db42d677c0a5c719a6956d8a7fc5fdcbf22a69837e`  
		Last Modified: Tue, 04 Oct 2022 20:13:30 GMT  
		Size: 157.8 MB (157822684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80571c0669f0277abd15b39422c7ac33098824b4e3acd5165a1094baff1c24a0`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce18cf0a5122414eb1417b6ea89e2af5dcbcfe8c8122f793c70530b5dfe185`  
		Last Modified: Tue, 04 Oct 2022 20:38:56 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6550656e761fb3dd33274b46efce609cf133d7ed5c3d2225307cb86e915686`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa241376abdf364b18ef913f22cd27f760430d56204f746263e788237ad2bc7b`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b0bbe614d6c4745bef5fb8c12ed68f7b5098aba644c3702b2c751772ff8dca`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83010d61e0e222aba800d09aa0e6f101273aa57850a02045c234cf45a46c26a`  
		Last Modified: Tue, 04 Oct 2022 20:38:54 GMT  
		Size: 1.8 MB (1834812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cece43f8685aa24f6224e5c09637d5766d50638f619e13f1ea4f6f5a6797992`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-builder-alpine`

```console
$ docker pull caddy@sha256:22a859f3d66929d869a26302a0acd2b8e2bcfb183a16037de3cb3a0b142bfae6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:8afe44a488e53c20b13d522ec0ceebf2f0574842e925f07709c4e3d0b34f95f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133500203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ef5b1bdbe7e51c149802adead793b95a3f4e9401df9c248dafef6e7294b9c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:16:54 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 21:18:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 21:18:32 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 21:18:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:18:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 21:18:32 GMT
WORKDIR /go
# Fri, 07 Oct 2022 04:35:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 04:35:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 04:35:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bccb3a1cff3b5f09bf1f21ba9ecb17c96329fb82f96605d922cfa4c9a82032`  
		Last Modified: Thu, 06 Oct 2022 21:25:08 GMT  
		Size: 122.3 MB (122251850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861cc3991b26fba6073631f27a1dc32bb27761195d912d05ee2f14b86fdf923f`  
		Last Modified: Thu, 06 Oct 2022 21:24:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f2801ecd75adee5f8c5111452c62dc9f74792e9de35771fdfaefcbe7a0004`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 6.9 MB (6941675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7494f25de5033fa48dcef9b9c880c76374b6d46092abb245fcd7ab1630c3bc`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 1.2 MB (1215177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8311897198e14fac14b1264d5fbc6cf8a02e580d706710353c401c0dcc67db`  
		Last Modified: Fri, 07 Oct 2022 04:35:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ceea5dfce2518bcd8f64951d0ff884bf4095037fb3ab84e81906b08889df2d4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8e6fb6b7549d30243de47d0ae0941d19a90e2f8240c24bdb7251033978fca3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:11:46 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:11:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:11:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:11:47 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:17:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:17:08 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:17:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:17:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:17:09 GMT
WORKDIR /go
# Sat, 08 Oct 2022 04:10:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 04:10:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 04:10:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 04:10:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b209b3d969f9a6352713d282fb4886bd906bc33154c9cc8af888e98292c36b82`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 284.7 KB (284689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3395a0d64b34009f33e3342948746a724fb68d28da16a8c474dcc6bd23b0c43`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f8b0abc05e00a9f055ae9fd2c0be61b1a031af3c0b983fde6989f6e51ad7e0`  
		Last Modified: Thu, 06 Oct 2022 20:33:21 GMT  
		Size: 118.6 MB (118635631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4ee43ba58df1ff51543e748374733cb56659f2f6cb2721e8bc55c9890bcd0`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f27e01fe424a71960c06a9bd9fdc198093ba0f8b341751f023e38129f1e52c`  
		Last Modified: Sat, 08 Oct 2022 04:11:06 GMT  
		Size: 6.8 MB (6808211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075d7a9278ef172ecaca28f1c74c6b1e45d8bfca5020998906df156bd9c93fdd`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 1.2 MB (1162977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f1f43b555f240d68b1d9f6fe17afdf4c78e8e165647d63558630489e43a713`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd54394bf4e39ecdbc7e7d3dc0ee1d3ec08689a5ad3f2a88563fe43a832d17e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab34ca7968e24f2883fb33f8c47da903cc3624ef5e9deb8e81fb8b51f537873`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:42:30 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:42:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 09:42:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:42:31 GMT
ENV GOLANG_VERSION=1.19.2
# Fri, 07 Oct 2022 09:49:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 07 Oct 2022 09:49:17 GMT
ENV GOPATH=/go
# Fri, 07 Oct 2022 09:49:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Oct 2022 09:49:18 GMT
WORKDIR /go
# Sat, 08 Oct 2022 05:06:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 05:06:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 05:06:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 05:06:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696b6cfba363e13486429ea964f92d832576e4e325397220afd2bff997ba045e`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 283.8 KB (283833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36573bb19dc804c15c8330b01de52ed6ded232a8b41d97998f1e33dee9f566a`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ebc5ada276c15274499e4bd347524b7eaaf42a3888a39db1464ecbaa94b9bf`  
		Last Modified: Fri, 07 Oct 2022 10:11:37 GMT  
		Size: 118.4 MB (118407461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5cc4edb1d1a08d0f82ac21910cc474b722bc371eaf97854b4bc90bc510ff00`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d7e71e64d4cde859c68147f4553124c90cf089314f225fdac27bb4729bc9c`  
		Last Modified: Sat, 08 Oct 2022 05:07:15 GMT  
		Size: 6.1 MB (6067873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf987d1eb410ed1530e75bbacb120d3efdc0437b5f68498cefae3d3245c4796`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800152f3498af5a4fbf7080d3044380f9826b5a1bf425001fa97d07ad544c736`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0ad855f7de2535a05dfc88f757a8ef1611a4578b85878ab2702e74994df4788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127986179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7396ddf3c1a000bdb6b5af6988bea71929050e5ea3c75b002f197fe6c6e25b9c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:48:18 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:48:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:48:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:48:21 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:49:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:49:56 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:49:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:49:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:49:59 GMT
WORKDIR /go
# Fri, 07 Oct 2022 08:01:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 08:01:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 08:01:29 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 08:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 08:01:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 08:01:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32db5db73116c723916b5df8f4ecc82d84f63f631c631d3fb81997d2fac11e9`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 284.5 KB (284532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c4b47475fc8104adcd7d897577b956078999e0cd332ec303fb21a18afcdf5c`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0598bfe6371f5c8223832079b9667d26a8bc5af5d1d818f5024e9c87d05a6`  
		Last Modified: Thu, 06 Oct 2022 20:57:08 GMT  
		Size: 116.8 MB (116820465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842c93ce66ef4b140121bbb9ec3badaa6b13b0f1a2a5a41e0bf5e4c8be8f852`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6608dc3160f80058977aa4f009e5ae9259e3278c7aa3ebf51ec2591c2090c`  
		Last Modified: Fri, 07 Oct 2022 08:02:20 GMT  
		Size: 7.1 MB (7052389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d63d110dcc7cc9d89ca5208169caa5cb389f3642ef114aead98e78606abc453`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3668944d647311a88fe8c1411dd9605faca9b1a213638d98ac647a5393f7adc6`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1750e31a6fb068abd57a4ca292cd0af0d488933c2286cc4fd3af92c7fd99702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128882306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e5ee9ab3729bc56e61c0311ee23fed2b88f72d89ead3e72ae4c1ce1369d99`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:26:03 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:28:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:28:54 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:28:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:28:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:28:56 GMT
WORKDIR /go
# Fri, 07 Oct 2022 07:56:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 07:56:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 07:56:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 07:56:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc648016b9956cdd58a13effd397263f1567720781730dc871f726e8cbf6dcb`  
		Last Modified: Thu, 06 Oct 2022 20:39:46 GMT  
		Size: 117.2 MB (117205225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c925b92d3e6aa9d43f83a9b3ea72790d539b1d983ddcffb8b95cf09a1e95e`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3131dd802f2ea71908bb86e0184679d69b9eccc01df8bd28eb998d3323d66063`  
		Last Modified: Fri, 07 Oct 2022 07:57:28 GMT  
		Size: 7.5 MB (7482443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82d9ca26c65fb5672a48eb58105343c6e06796084b0599b13f858bf22efbbd`  
		Last Modified: Fri, 07 Oct 2022 07:57:27 GMT  
		Size: 1.1 MB (1103855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396418b7a946c59b42806f6c5dcb72b12da6296dde780614b39c0733e2d5f6f`  
		Last Modified: Fri, 07 Oct 2022 07:57:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4babe26aa4db963e2c1ba319a0f8e9a96c54a10c46dde7d0222f1889fe055d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131829172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e088de34239daf3a02ff2b831d410cbd9ef7c66fbeffc20a99f578027e437853`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:16:12 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:18:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:18:43 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:18:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:18:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:18:44 GMT
WORKDIR /go
# Fri, 07 Oct 2022 10:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 10:24:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 10:24:28 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 10:24:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 10:24:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 10:24:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3229342a30d3f1b9300228f7e3414e521024d8294398cc78d68c228dc8d1c40`  
		Last Modified: Thu, 06 Oct 2022 20:27:07 GMT  
		Size: 120.7 MB (120732457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e365613c053faa0517c5a9a3a8561d8dc4efe2d2d1159866dae02b07eb9f38d3`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca88f390fc5368bde96f7ab5aefec4cc5b192f7a443dc75ba03f35657b6ef4`  
		Last Modified: Fri, 07 Oct 2022 10:25:25 GMT  
		Size: 7.1 MB (7053036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2a2b0715c0c7b6eb7481142dfbc5e20109831c91458b10da2c70fb1c5a93fe`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 1.2 MB (1167415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad9784cee46592eb85a25958acb5461a20bdc2ce52e0d09405dcc330288022`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f6c3f33dda0aad41a0d698c876064a5aca204d85fb603e864d89b065f92014cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:2.6.1-builder-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:fce8cf0a954111a1cb7e15ec8c9cf74dec576c92059e0a9cd3dadedffeee1cfb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888597946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67b82a73ab94a2525eb495091fbc693b28af993fc6cafbb3768c824f32acf18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:44:27 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:02 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:49:04 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:35:50 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:07 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c61bfb24309aadc8d001a8f706cedd3583ce2125fb7bc1628b7a83cfc7bb33`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e32dad104a4eff9e37934f63302fd3fa0226a9bdca330621819352ea66c94`  
		Last Modified: Tue, 04 Oct 2022 20:14:22 GMT  
		Size: 157.6 MB (157622445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f32605b45357608ad3962e2c0e0b6a16950c0958e61a5ea142b25f285bb21`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf8da2a2b79782e508e1f0cb603dc595be9caf18e69e6d38f5d00b4ddcc68f`  
		Last Modified: Tue, 04 Oct 2022 20:38:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724ca131e07cfb838c3f0fcfb2a103ce9b4f53dd0192aa29dcc63d376a10ba1`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d742c8bb37a68aed95adcd87d5288c1b3cd6f125cbe580316071c24e6dabd`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db91b0bb8cd4047b2e49a3be46d6ba19d1310228b61c3ad19969a9e2b0af5d6`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e44bf097cee24852462f4634e99e2f7620b77dc3842d687791c926c5a48de56`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.6 MB (1630878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bfff7b454e1e2bbc5b8cfff2ace2a606e33a84bb251fd6edc3e906e6addbe`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:482053b6811d642bb974423087fbf568468ffc9cf170dac246d1ff6779177eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `caddy:2.6.1-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:ca9809a34b96a52e7e6eeef8d2057c1ba1a1a601eec7d91189d4b28e04573019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532828578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430f6ae7d3a4c215ba209863ecea0ab3685b63ad0aba36bf2b83eb90958b4ac8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:48:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:48:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:48:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:48:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:49:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:49:30 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:49:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:40:59 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:44:14 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:44:16 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:37:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:37:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:37:19 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:37:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6316baacdbe5997d732fa3555c0cd6f52fd467b41d4d41b596d460cfe8aa`  
		Last Modified: Wed, 14 Sep 2022 13:23:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de847c6f89452694f7278d29e3920062ee79faf74467742e329a71dc1db8805`  
		Last Modified: Wed, 14 Sep 2022 13:23:32 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1a6aca4358241a5ae1012bcd11240db54df9849aa25d07166c302dd3014dee`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0740ce986dad4039bc222ec6cfe798adfe4573d313d4e3583b8694109298e`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ed2e7f7ad8700539fdcbbfa0a73ce470c9b68aad955ee06135135e35f19d3`  
		Last Modified: Wed, 14 Sep 2022 13:23:39 GMT  
		Size: 25.7 MB (25676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde228a76aaef32add4bb50c16be55584a1328125aa2b2436d22da9d311837a4`  
		Last Modified: Wed, 14 Sep 2022 13:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab59b5ad3cb6d91ad9c3a3064155bffbd0cafff4fa66dc0d04e68d873a23c2c9`  
		Last Modified: Wed, 14 Sep 2022 13:23:29 GMT  
		Size: 526.6 KB (526562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7b60da979d12d87db1ff1c51bfbdabdf15744a9fc23c48d1f527d0d64a525`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915d3981a43f92982ff6e6db42d677c0a5c719a6956d8a7fc5fdcbf22a69837e`  
		Last Modified: Tue, 04 Oct 2022 20:13:30 GMT  
		Size: 157.8 MB (157822684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80571c0669f0277abd15b39422c7ac33098824b4e3acd5165a1094baff1c24a0`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce18cf0a5122414eb1417b6ea89e2af5dcbcfe8c8122f793c70530b5dfe185`  
		Last Modified: Tue, 04 Oct 2022 20:38:56 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6550656e761fb3dd33274b46efce609cf133d7ed5c3d2225307cb86e915686`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa241376abdf364b18ef913f22cd27f760430d56204f746263e788237ad2bc7b`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b0bbe614d6c4745bef5fb8c12ed68f7b5098aba644c3702b2c751772ff8dca`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83010d61e0e222aba800d09aa0e6f101273aa57850a02045c234cf45a46c26a`  
		Last Modified: Tue, 04 Oct 2022 20:38:54 GMT  
		Size: 1.8 MB (1834812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cece43f8685aa24f6224e5c09637d5766d50638f619e13f1ea4f6f5a6797992`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-windowsservercore`

```console
$ docker pull caddy@sha256:a2f4650d657ce94148fda7db712cc27b1cf037cd53535cdcfe6021488cb35680
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:2.6.1-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-windowsservercore` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f65a2a6e954346897215a9d2fa42d57afe06720d80aa6f5ee846aea9dd2343e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:2.6.1-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:391c3e9d6a79f66b9cfdc3800ac89da113665ef28bd627bc2ae077a8fdffa0d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `caddy:2.6.1-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:75d2e29d0c3ec9aa78e640c022d5afec48c2c8ccefe0f956280f66bcced7cceb
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
$ docker pull caddy@sha256:5e68e231a2fb583cc2bafe472844495cd9c1b119b626cb61777a75f990886906
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181f13e1cc5fd90d0b4869e57689b5200589ca1029971fc7233082c04806a55b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 04:34:57 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:34:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 04:34:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 04:35:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 04:35:01 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 04:35:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890b94b17a6b1f257ddec10a103ff342db99516b0d339260623d6610db9b1349`  
		Last Modified: Fri, 07 Oct 2022 04:35:27 GMT  
		Size: 14.5 MB (14493818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d852ea4bd9f60570e83e432bcb361e0400dc3b2c3a264a447dfc2f6b292c0a`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:12eface0625a91f60ec1e6f8ccd864d52c9dc69f3b02ea126e4fdaacf8de5bd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0d4211357adf7a3124613f982947e3745803a9205db56b524ae70f1f03f521`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 04:09:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 08 Oct 2022 04:09:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Sat, 08 Oct 2022 04:09:55 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:09:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 08 Oct 2022 04:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 80
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443/udp
# Sat, 08 Oct 2022 04:10:00 GMT
EXPOSE 2019
# Sat, 08 Oct 2022 04:10:00 GMT
WORKDIR /srv
# Sat, 08 Oct 2022 04:10:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa0e79d89709c451dcc1ed2799b94c19204fb58ea7cce7895eef1f51c01bb50`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 304.5 KB (304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9215626c7fc1bfbffb15114b3a5de7fc64de1e7a2a21ee2056121f5ef65b2338`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ca8b546a2bb8c3467ac3eafdca5479dd6396e518b348315a1b16a18519b61`  
		Last Modified: Sat, 08 Oct 2022 04:10:49 GMT  
		Size: 13.8 MB (13848654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e20fa1676a89097bb7bfd9deb83ec1b2ba35972a2c365e7e0b111bf46a430`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8c5c01339078f89f85a5a7cd08d8bd89962900d295af83cc0eb70de31c4d51ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c275d9a5ca87dde16a12a6d524b9a542b9e77e96ead14f8c577857b6091f24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:17:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:17:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:17:46 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:17:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:17:52 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:17:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11d99bb68cba432782c86e461f4c830d8bc08ba0b2df2999db3ab67a55f57e`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 303.6 KB (303619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30dd3a0b20a2d25c12f53bf9ae92037f177e924b7613dbbeedca0029d44215`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0645b8aab72e227505345e7745508a1f23ed2ff304884458f31d828eac843`  
		Last Modified: Fri, 07 Oct 2022 07:18:46 GMT  
		Size: 13.8 MB (13824551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978d7d8e43141c7a175739d7aafcb64b5b8f6561efb3295d91c186bfab20eb3`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e6d1ad533fd36cd36a387471e708740876c809760795f8868490beab7d98443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1814d3a7f6c971e84b565c46272fc51961c9e67e0e8787781be733c087a22`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 08:00:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 08:00:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 08:00:59 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 08:01:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 08:01:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 08:01:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 08:01:06 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 08:01:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 08:01:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 08:01:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 08:01:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 08:01:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 08:01:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 08:01:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 08:01:14 GMT
EXPOSE 80
# Fri, 07 Oct 2022 08:01:15 GMT
EXPOSE 443
# Fri, 07 Oct 2022 08:01:16 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 08:01:17 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 08:01:18 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 08:01:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6fca9d7511cb60edf3b5df387d6b1fd5aaac17867575fc733cf40137b95a90`  
		Last Modified: Fri, 07 Oct 2022 08:02:04 GMT  
		Size: 304.3 KB (304303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8483ebae1fd52b4e5a413ddd322fedfc3978bd5f95dfd62ea2c53f1a0b7a7e05`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ad12dc08ecd5447289e06895740be336d526d7bec274b5cab707b3be6c4df`  
		Last Modified: Fri, 07 Oct 2022 08:02:05 GMT  
		Size: 13.2 MB (13196260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b783a84a1d985b8c4d150880a665dffed5e8d3cd282ed0f45af0b28e45c30a`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:3c296624df3a6ffb31e3a5eca10b509c80150fe12e9b19ebf27e061189d44278
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4250b6ab2344a47d567b072f8080c8f6aa93b04bd773b51fa57148ac08e30379`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:56:13 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:56:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:56:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:56:22 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:56:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d070e557e928b65136b4bb037dd73ddfb5be784310db1f0f3640ce1216afc`  
		Last Modified: Fri, 07 Oct 2022 07:57:11 GMT  
		Size: 12.9 MB (12853693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40adebe65a7cbe002c94177299a2ae8a216f554d7d6ae5eec0916ba7330da421`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3e5aa9861d4d5e9c0dfda105fa0b598ee20d5f254b734f5a418c99f6a5b9b5af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2a3441daa59cefaa1dbb6d0edd094f53abe4b3c89877fd3b7121dd53d15ef3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 10:23:51 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:23:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 10:24:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 10:24:04 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 10:24:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 10:24:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 10:24:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 10:24:09 GMT
EXPOSE 80
# Fri, 07 Oct 2022 10:24:10 GMT
EXPOSE 443
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 10:24:12 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 10:24:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8c37b8106cb4218c6396b95deabef48406b60274cd3304a53e50b645cd9e7`  
		Last Modified: Fri, 07 Oct 2022 10:25:13 GMT  
		Size: 14.0 MB (14001566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334954d04c67d43f4bab0b7774053bae33c535a25cc073cf20528174bf6031e9`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:88717c434912a73202d619948c3352c352ada39682e290da1f669685783ea910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:8afe44a488e53c20b13d522ec0ceebf2f0574842e925f07709c4e3d0b34f95f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133500203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ef5b1bdbe7e51c149802adead793b95a3f4e9401df9c248dafef6e7294b9c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:16:54 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 21:18:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 21:18:32 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 21:18:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:18:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 21:18:32 GMT
WORKDIR /go
# Fri, 07 Oct 2022 04:35:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 04:35:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 04:35:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bccb3a1cff3b5f09bf1f21ba9ecb17c96329fb82f96605d922cfa4c9a82032`  
		Last Modified: Thu, 06 Oct 2022 21:25:08 GMT  
		Size: 122.3 MB (122251850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861cc3991b26fba6073631f27a1dc32bb27761195d912d05ee2f14b86fdf923f`  
		Last Modified: Thu, 06 Oct 2022 21:24:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f2801ecd75adee5f8c5111452c62dc9f74792e9de35771fdfaefcbe7a0004`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 6.9 MB (6941675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7494f25de5033fa48dcef9b9c880c76374b6d46092abb245fcd7ab1630c3bc`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 1.2 MB (1215177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8311897198e14fac14b1264d5fbc6cf8a02e580d706710353c401c0dcc67db`  
		Last Modified: Fri, 07 Oct 2022 04:35:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ceea5dfce2518bcd8f64951d0ff884bf4095037fb3ab84e81906b08889df2d4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8e6fb6b7549d30243de47d0ae0941d19a90e2f8240c24bdb7251033978fca3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:11:46 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:11:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:11:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:11:47 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:17:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:17:08 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:17:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:17:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:17:09 GMT
WORKDIR /go
# Sat, 08 Oct 2022 04:10:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 04:10:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 04:10:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 04:10:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b209b3d969f9a6352713d282fb4886bd906bc33154c9cc8af888e98292c36b82`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 284.7 KB (284689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3395a0d64b34009f33e3342948746a724fb68d28da16a8c474dcc6bd23b0c43`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f8b0abc05e00a9f055ae9fd2c0be61b1a031af3c0b983fde6989f6e51ad7e0`  
		Last Modified: Thu, 06 Oct 2022 20:33:21 GMT  
		Size: 118.6 MB (118635631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4ee43ba58df1ff51543e748374733cb56659f2f6cb2721e8bc55c9890bcd0`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f27e01fe424a71960c06a9bd9fdc198093ba0f8b341751f023e38129f1e52c`  
		Last Modified: Sat, 08 Oct 2022 04:11:06 GMT  
		Size: 6.8 MB (6808211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075d7a9278ef172ecaca28f1c74c6b1e45d8bfca5020998906df156bd9c93fdd`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 1.2 MB (1162977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f1f43b555f240d68b1d9f6fe17afdf4c78e8e165647d63558630489e43a713`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd54394bf4e39ecdbc7e7d3dc0ee1d3ec08689a5ad3f2a88563fe43a832d17e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab34ca7968e24f2883fb33f8c47da903cc3624ef5e9deb8e81fb8b51f537873`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:42:30 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:42:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 09:42:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:42:31 GMT
ENV GOLANG_VERSION=1.19.2
# Fri, 07 Oct 2022 09:49:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 07 Oct 2022 09:49:17 GMT
ENV GOPATH=/go
# Fri, 07 Oct 2022 09:49:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Oct 2022 09:49:18 GMT
WORKDIR /go
# Sat, 08 Oct 2022 05:06:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 05:06:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 05:06:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 05:06:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696b6cfba363e13486429ea964f92d832576e4e325397220afd2bff997ba045e`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 283.8 KB (283833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36573bb19dc804c15c8330b01de52ed6ded232a8b41d97998f1e33dee9f566a`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ebc5ada276c15274499e4bd347524b7eaaf42a3888a39db1464ecbaa94b9bf`  
		Last Modified: Fri, 07 Oct 2022 10:11:37 GMT  
		Size: 118.4 MB (118407461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5cc4edb1d1a08d0f82ac21910cc474b722bc371eaf97854b4bc90bc510ff00`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d7e71e64d4cde859c68147f4553124c90cf089314f225fdac27bb4729bc9c`  
		Last Modified: Sat, 08 Oct 2022 05:07:15 GMT  
		Size: 6.1 MB (6067873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf987d1eb410ed1530e75bbacb120d3efdc0437b5f68498cefae3d3245c4796`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800152f3498af5a4fbf7080d3044380f9826b5a1bf425001fa97d07ad544c736`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0ad855f7de2535a05dfc88f757a8ef1611a4578b85878ab2702e74994df4788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127986179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7396ddf3c1a000bdb6b5af6988bea71929050e5ea3c75b002f197fe6c6e25b9c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:48:18 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:48:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:48:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:48:21 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:49:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:49:56 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:49:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:49:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:49:59 GMT
WORKDIR /go
# Fri, 07 Oct 2022 08:01:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 08:01:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 08:01:29 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 08:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 08:01:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 08:01:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32db5db73116c723916b5df8f4ecc82d84f63f631c631d3fb81997d2fac11e9`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 284.5 KB (284532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c4b47475fc8104adcd7d897577b956078999e0cd332ec303fb21a18afcdf5c`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0598bfe6371f5c8223832079b9667d26a8bc5af5d1d818f5024e9c87d05a6`  
		Last Modified: Thu, 06 Oct 2022 20:57:08 GMT  
		Size: 116.8 MB (116820465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842c93ce66ef4b140121bbb9ec3badaa6b13b0f1a2a5a41e0bf5e4c8be8f852`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6608dc3160f80058977aa4f009e5ae9259e3278c7aa3ebf51ec2591c2090c`  
		Last Modified: Fri, 07 Oct 2022 08:02:20 GMT  
		Size: 7.1 MB (7052389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d63d110dcc7cc9d89ca5208169caa5cb389f3642ef114aead98e78606abc453`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3668944d647311a88fe8c1411dd9605faca9b1a213638d98ac647a5393f7adc6`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:1750e31a6fb068abd57a4ca292cd0af0d488933c2286cc4fd3af92c7fd99702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128882306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e5ee9ab3729bc56e61c0311ee23fed2b88f72d89ead3e72ae4c1ce1369d99`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:26:03 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:28:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:28:54 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:28:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:28:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:28:56 GMT
WORKDIR /go
# Fri, 07 Oct 2022 07:56:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 07:56:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 07:56:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 07:56:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc648016b9956cdd58a13effd397263f1567720781730dc871f726e8cbf6dcb`  
		Last Modified: Thu, 06 Oct 2022 20:39:46 GMT  
		Size: 117.2 MB (117205225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c925b92d3e6aa9d43f83a9b3ea72790d539b1d983ddcffb8b95cf09a1e95e`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3131dd802f2ea71908bb86e0184679d69b9eccc01df8bd28eb998d3323d66063`  
		Last Modified: Fri, 07 Oct 2022 07:57:28 GMT  
		Size: 7.5 MB (7482443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82d9ca26c65fb5672a48eb58105343c6e06796084b0599b13f858bf22efbbd`  
		Last Modified: Fri, 07 Oct 2022 07:57:27 GMT  
		Size: 1.1 MB (1103855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396418b7a946c59b42806f6c5dcb72b12da6296dde780614b39c0733e2d5f6f`  
		Last Modified: Fri, 07 Oct 2022 07:57:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:4babe26aa4db963e2c1ba319a0f8e9a96c54a10c46dde7d0222f1889fe055d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131829172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e088de34239daf3a02ff2b831d410cbd9ef7c66fbeffc20a99f578027e437853`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:16:12 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:18:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:18:43 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:18:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:18:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:18:44 GMT
WORKDIR /go
# Fri, 07 Oct 2022 10:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 10:24:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 10:24:28 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 10:24:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 10:24:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 10:24:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3229342a30d3f1b9300228f7e3414e521024d8294398cc78d68c228dc8d1c40`  
		Last Modified: Thu, 06 Oct 2022 20:27:07 GMT  
		Size: 120.7 MB (120732457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e365613c053faa0517c5a9a3a8561d8dc4efe2d2d1159866dae02b07eb9f38d3`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca88f390fc5368bde96f7ab5aefec4cc5b192f7a443dc75ba03f35657b6ef4`  
		Last Modified: Fri, 07 Oct 2022 10:25:25 GMT  
		Size: 7.1 MB (7053036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2a2b0715c0c7b6eb7481142dfbc5e20109831c91458b10da2c70fb1c5a93fe`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 1.2 MB (1167415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad9784cee46592eb85a25958acb5461a20bdc2ce52e0d09405dcc330288022`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:fce8cf0a954111a1cb7e15ec8c9cf74dec576c92059e0a9cd3dadedffeee1cfb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888597946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67b82a73ab94a2525eb495091fbc693b28af993fc6cafbb3768c824f32acf18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:44:27 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:02 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:49:04 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:35:50 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:07 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c61bfb24309aadc8d001a8f706cedd3583ce2125fb7bc1628b7a83cfc7bb33`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e32dad104a4eff9e37934f63302fd3fa0226a9bdca330621819352ea66c94`  
		Last Modified: Tue, 04 Oct 2022 20:14:22 GMT  
		Size: 157.6 MB (157622445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f32605b45357608ad3962e2c0e0b6a16950c0958e61a5ea142b25f285bb21`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf8da2a2b79782e508e1f0cb603dc595be9caf18e69e6d38f5d00b4ddcc68f`  
		Last Modified: Tue, 04 Oct 2022 20:38:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724ca131e07cfb838c3f0fcfb2a103ce9b4f53dd0192aa29dcc63d376a10ba1`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d742c8bb37a68aed95adcd87d5288c1b3cd6f125cbe580316071c24e6dabd`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db91b0bb8cd4047b2e49a3be46d6ba19d1310228b61c3ad19969a9e2b0af5d6`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e44bf097cee24852462f4634e99e2f7620b77dc3842d687791c926c5a48de56`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.6 MB (1630878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bfff7b454e1e2bbc5b8cfff2ace2a606e33a84bb251fd6edc3e906e6addbe`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:ca9809a34b96a52e7e6eeef8d2057c1ba1a1a601eec7d91189d4b28e04573019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532828578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430f6ae7d3a4c215ba209863ecea0ab3685b63ad0aba36bf2b83eb90958b4ac8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:48:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:48:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:48:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:48:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:49:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:49:30 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:49:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:40:59 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:44:14 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:44:16 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:37:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:37:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:37:19 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:37:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6316baacdbe5997d732fa3555c0cd6f52fd467b41d4d41b596d460cfe8aa`  
		Last Modified: Wed, 14 Sep 2022 13:23:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de847c6f89452694f7278d29e3920062ee79faf74467742e329a71dc1db8805`  
		Last Modified: Wed, 14 Sep 2022 13:23:32 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1a6aca4358241a5ae1012bcd11240db54df9849aa25d07166c302dd3014dee`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0740ce986dad4039bc222ec6cfe798adfe4573d313d4e3583b8694109298e`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ed2e7f7ad8700539fdcbbfa0a73ce470c9b68aad955ee06135135e35f19d3`  
		Last Modified: Wed, 14 Sep 2022 13:23:39 GMT  
		Size: 25.7 MB (25676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde228a76aaef32add4bb50c16be55584a1328125aa2b2436d22da9d311837a4`  
		Last Modified: Wed, 14 Sep 2022 13:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab59b5ad3cb6d91ad9c3a3064155bffbd0cafff4fa66dc0d04e68d873a23c2c9`  
		Last Modified: Wed, 14 Sep 2022 13:23:29 GMT  
		Size: 526.6 KB (526562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7b60da979d12d87db1ff1c51bfbdabdf15744a9fc23c48d1f527d0d64a525`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915d3981a43f92982ff6e6db42d677c0a5c719a6956d8a7fc5fdcbf22a69837e`  
		Last Modified: Tue, 04 Oct 2022 20:13:30 GMT  
		Size: 157.8 MB (157822684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80571c0669f0277abd15b39422c7ac33098824b4e3acd5165a1094baff1c24a0`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce18cf0a5122414eb1417b6ea89e2af5dcbcfe8c8122f793c70530b5dfe185`  
		Last Modified: Tue, 04 Oct 2022 20:38:56 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6550656e761fb3dd33274b46efce609cf133d7ed5c3d2225307cb86e915686`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa241376abdf364b18ef913f22cd27f760430d56204f746263e788237ad2bc7b`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b0bbe614d6c4745bef5fb8c12ed68f7b5098aba644c3702b2c751772ff8dca`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83010d61e0e222aba800d09aa0e6f101273aa57850a02045c234cf45a46c26a`  
		Last Modified: Tue, 04 Oct 2022 20:38:54 GMT  
		Size: 1.8 MB (1834812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cece43f8685aa24f6224e5c09637d5766d50638f619e13f1ea4f6f5a6797992`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:22a859f3d66929d869a26302a0acd2b8e2bcfb183a16037de3cb3a0b142bfae6
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
$ docker pull caddy@sha256:8afe44a488e53c20b13d522ec0ceebf2f0574842e925f07709c4e3d0b34f95f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133500203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ef5b1bdbe7e51c149802adead793b95a3f4e9401df9c248dafef6e7294b9c3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:16:54 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 21:18:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 21:18:32 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 21:18:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 21:18:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 21:18:32 GMT
WORKDIR /go
# Fri, 07 Oct 2022 04:35:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:35:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 04:35:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 04:35:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 04:35:07 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bccb3a1cff3b5f09bf1f21ba9ecb17c96329fb82f96605d922cfa4c9a82032`  
		Last Modified: Thu, 06 Oct 2022 21:25:08 GMT  
		Size: 122.3 MB (122251850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861cc3991b26fba6073631f27a1dc32bb27761195d912d05ee2f14b86fdf923f`  
		Last Modified: Thu, 06 Oct 2022 21:24:51 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f2801ecd75adee5f8c5111452c62dc9f74792e9de35771fdfaefcbe7a0004`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 6.9 MB (6941675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7494f25de5033fa48dcef9b9c880c76374b6d46092abb245fcd7ab1630c3bc`  
		Last Modified: Fri, 07 Oct 2022 04:35:39 GMT  
		Size: 1.2 MB (1215177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8311897198e14fac14b1264d5fbc6cf8a02e580d706710353c401c0dcc67db`  
		Last Modified: Fri, 07 Oct 2022 04:35:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:ceea5dfce2518bcd8f64951d0ff884bf4095037fb3ab84e81906b08889df2d4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8e6fb6b7549d30243de47d0ae0941d19a90e2f8240c24bdb7251033978fca3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:11:46 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:11:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:11:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:11:47 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:17:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:17:08 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:17:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:17:09 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:17:09 GMT
WORKDIR /go
# Sat, 08 Oct 2022 04:10:09 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:10:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 04:10:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 04:10:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 04:10:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b209b3d969f9a6352713d282fb4886bd906bc33154c9cc8af888e98292c36b82`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 284.7 KB (284689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3395a0d64b34009f33e3342948746a724fb68d28da16a8c474dcc6bd23b0c43`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f8b0abc05e00a9f055ae9fd2c0be61b1a031af3c0b983fde6989f6e51ad7e0`  
		Last Modified: Thu, 06 Oct 2022 20:33:21 GMT  
		Size: 118.6 MB (118635631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4ee43ba58df1ff51543e748374733cb56659f2f6cb2721e8bc55c9890bcd0`  
		Last Modified: Thu, 06 Oct 2022 20:32:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f27e01fe424a71960c06a9bd9fdc198093ba0f8b341751f023e38129f1e52c`  
		Last Modified: Sat, 08 Oct 2022 04:11:06 GMT  
		Size: 6.8 MB (6808211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075d7a9278ef172ecaca28f1c74c6b1e45d8bfca5020998906df156bd9c93fdd`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 1.2 MB (1162977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f1f43b555f240d68b1d9f6fe17afdf4c78e8e165647d63558630489e43a713`  
		Last Modified: Sat, 08 Oct 2022 04:11:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:bd54394bf4e39ecdbc7e7d3dc0ee1d3ec08689a5ad3f2a88563fe43a832d17e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab34ca7968e24f2883fb33f8c47da903cc3624ef5e9deb8e81fb8b51f537873`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:42:30 GMT
RUN apk add --no-cache ca-certificates
# Fri, 07 Oct 2022 09:42:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 09:42:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:42:31 GMT
ENV GOLANG_VERSION=1.19.2
# Fri, 07 Oct 2022 09:49:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 07 Oct 2022 09:49:17 GMT
ENV GOPATH=/go
# Fri, 07 Oct 2022 09:49:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:49:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Oct 2022 09:49:18 GMT
WORKDIR /go
# Sat, 08 Oct 2022 05:06:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_VERSION=v0.3.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 05:06:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 08 Oct 2022 05:06:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 08 Oct 2022 05:06:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 08 Oct 2022 05:06:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696b6cfba363e13486429ea964f92d832576e4e325397220afd2bff997ba045e`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 283.8 KB (283833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36573bb19dc804c15c8330b01de52ed6ded232a8b41d97998f1e33dee9f566a`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ebc5ada276c15274499e4bd347524b7eaaf42a3888a39db1464ecbaa94b9bf`  
		Last Modified: Fri, 07 Oct 2022 10:11:37 GMT  
		Size: 118.4 MB (118407461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5cc4edb1d1a08d0f82ac21910cc474b722bc371eaf97854b4bc90bc510ff00`  
		Last Modified: Fri, 07 Oct 2022 10:11:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d7e71e64d4cde859c68147f4553124c90cf089314f225fdac27bb4729bc9c`  
		Last Modified: Sat, 08 Oct 2022 05:07:15 GMT  
		Size: 6.1 MB (6067873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf987d1eb410ed1530e75bbacb120d3efdc0437b5f68498cefae3d3245c4796`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800152f3498af5a4fbf7080d3044380f9826b5a1bf425001fa97d07ad544c736`  
		Last Modified: Sat, 08 Oct 2022 05:07:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0ad855f7de2535a05dfc88f757a8ef1611a4578b85878ab2702e74994df4788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127986179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7396ddf3c1a000bdb6b5af6988bea71929050e5ea3c75b002f197fe6c6e25b9c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:48:18 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:48:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:48:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:48:21 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:49:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:49:56 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:49:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:49:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:49:59 GMT
WORKDIR /go
# Fri, 07 Oct 2022 08:01:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 08:01:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 08:01:29 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 08:01:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 08:01:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 08:01:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32db5db73116c723916b5df8f4ecc82d84f63f631c631d3fb81997d2fac11e9`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 284.5 KB (284532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c4b47475fc8104adcd7d897577b956078999e0cd332ec303fb21a18afcdf5c`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd0598bfe6371f5c8223832079b9667d26a8bc5af5d1d818f5024e9c87d05a6`  
		Last Modified: Thu, 06 Oct 2022 20:57:08 GMT  
		Size: 116.8 MB (116820465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842c93ce66ef4b140121bbb9ec3badaa6b13b0f1a2a5a41e0bf5e4c8be8f852`  
		Last Modified: Thu, 06 Oct 2022 20:56:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d6608dc3160f80058977aa4f009e5ae9259e3278c7aa3ebf51ec2591c2090c`  
		Last Modified: Fri, 07 Oct 2022 08:02:20 GMT  
		Size: 7.1 MB (7052389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d63d110dcc7cc9d89ca5208169caa5cb389f3642ef114aead98e78606abc453`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 1.1 MB (1120444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3668944d647311a88fe8c1411dd9605faca9b1a213638d98ac647a5393f7adc6`  
		Last Modified: Fri, 07 Oct 2022 08:02:19 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1750e31a6fb068abd57a4ca292cd0af0d488933c2286cc4fd3af92c7fd99702b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128882306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50e5ee9ab3729bc56e61c0311ee23fed2b88f72d89ead3e72ae4c1ce1369d99`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:26:03 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:28:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:28:54 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:28:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:28:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:28:56 GMT
WORKDIR /go
# Fri, 07 Oct 2022 07:56:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 07:56:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 07:56:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 07:56:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc648016b9956cdd58a13effd397263f1567720781730dc871f726e8cbf6dcb`  
		Last Modified: Thu, 06 Oct 2022 20:39:46 GMT  
		Size: 117.2 MB (117205225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c925b92d3e6aa9d43f83a9b3ea72790d539b1d983ddcffb8b95cf09a1e95e`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3131dd802f2ea71908bb86e0184679d69b9eccc01df8bd28eb998d3323d66063`  
		Last Modified: Fri, 07 Oct 2022 07:57:28 GMT  
		Size: 7.5 MB (7482443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82d9ca26c65fb5672a48eb58105343c6e06796084b0599b13f858bf22efbbd`  
		Last Modified: Fri, 07 Oct 2022 07:57:27 GMT  
		Size: 1.1 MB (1103855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a396418b7a946c59b42806f6c5dcb72b12da6296dde780614b39c0733e2d5f6f`  
		Last Modified: Fri, 07 Oct 2022 07:57:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4babe26aa4db963e2c1ba319a0f8e9a96c54a10c46dde7d0222f1889fe055d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131829172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e088de34239daf3a02ff2b831d410cbd9ef7c66fbeffc20a99f578027e437853`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:16:12 GMT
ENV GOLANG_VERSION=1.19.2
# Thu, 06 Oct 2022 20:18:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Oct 2022 20:18:43 GMT
ENV GOPATH=/go
# Thu, 06 Oct 2022 20:18:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 20:18:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Oct 2022 20:18:44 GMT
WORKDIR /go
# Fri, 07 Oct 2022 10:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Oct 2022 10:24:28 GMT
ENV XCADDY_VERSION=v0.3.1
# Fri, 07 Oct 2022 10:24:28 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Oct 2022 10:24:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Oct 2022 10:24:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Oct 2022 10:24:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3229342a30d3f1b9300228f7e3414e521024d8294398cc78d68c228dc8d1c40`  
		Last Modified: Thu, 06 Oct 2022 20:27:07 GMT  
		Size: 120.7 MB (120732457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e365613c053faa0517c5a9a3a8561d8dc4efe2d2d1159866dae02b07eb9f38d3`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca88f390fc5368bde96f7ab5aefec4cc5b192f7a443dc75ba03f35657b6ef4`  
		Last Modified: Fri, 07 Oct 2022 10:25:25 GMT  
		Size: 7.1 MB (7053036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2a2b0715c0c7b6eb7481142dfbc5e20109831c91458b10da2c70fb1c5a93fe`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 1.2 MB (1167415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad9784cee46592eb85a25958acb5461a20bdc2ce52e0d09405dcc330288022`  
		Last Modified: Fri, 07 Oct 2022 10:25:24 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f6c3f33dda0aad41a0d698c876064a5aca204d85fb603e864d89b065f92014cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:fce8cf0a954111a1cb7e15ec8c9cf74dec576c92059e0a9cd3dadedffeee1cfb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888597946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67b82a73ab94a2525eb495091fbc693b28af993fc6cafbb3768c824f32acf18`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:53:02 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:53:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:53:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:53:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:54:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:54:42 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:55:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:44:27 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:02 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:49:04 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:35:50 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:35:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:05 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:07 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46cb21791119f57fee8356ecd2742ee657e38fda347b5aaf1ab82c5257f6ab4`  
		Last Modified: Wed, 14 Sep 2022 13:24:35 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a233492809d7d153ccc1ce383a93179a683b56b80691bdd2803df9701f7cd76`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1203c125a81e64fe38de87dbdb26d0811fbf889428ea5d1b0d53502db44903`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c9e858188aa75d29a703f3709dbeb4002b8bfc1b37090a1ef2656630d7c7a`  
		Last Modified: Wed, 14 Sep 2022 13:24:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595aefee200f2e098dc894968e32799b6514b87e5000abb60bf9cd77ba04f41`  
		Last Modified: Wed, 14 Sep 2022 13:24:38 GMT  
		Size: 25.4 MB (25446607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a242828d90d404c6bf0aedeff32d4affe77cd43ebb7ad0c7bb535420f728f5`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f9452c9b0bb0321568934d2581a61b4a3e7b7e536a2666e8f27f34146fe66`  
		Last Modified: Wed, 14 Sep 2022 13:24:28 GMT  
		Size: 315.5 KB (315491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c61bfb24309aadc8d001a8f706cedd3583ce2125fb7bc1628b7a83cfc7bb33`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e32dad104a4eff9e37934f63302fd3fa0226a9bdca330621819352ea66c94`  
		Last Modified: Tue, 04 Oct 2022 20:14:22 GMT  
		Size: 157.6 MB (157622445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69f32605b45357608ad3962e2c0e0b6a16950c0958e61a5ea142b25f285bb21`  
		Last Modified: Tue, 04 Oct 2022 20:13:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf8da2a2b79782e508e1f0cb603dc595be9caf18e69e6d38f5d00b4ddcc68f`  
		Last Modified: Tue, 04 Oct 2022 20:38:39 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724ca131e07cfb838c3f0fcfb2a103ce9b4f53dd0192aa29dcc63d376a10ba1`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11d742c8bb37a68aed95adcd87d5288c1b3cd6f125cbe580316071c24e6dabd`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db91b0bb8cd4047b2e49a3be46d6ba19d1310228b61c3ad19969a9e2b0af5d6`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e44bf097cee24852462f4634e99e2f7620b77dc3842d687791c926c5a48de56`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.6 MB (1630878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0bfff7b454e1e2bbc5b8cfff2ace2a606e33a84bb251fd6edc3e906e6addbe`  
		Last Modified: Tue, 04 Oct 2022 20:38:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:482053b6811d642bb974423087fbf568468ffc9cf170dac246d1ff6779177eab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:ca9809a34b96a52e7e6eeef8d2057c1ba1a1a601eec7d91189d4b28e04573019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532828578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430f6ae7d3a4c215ba209863ecea0ab3685b63ad0aba36bf2b83eb90958b4ac8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 12:48:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 14 Sep 2022 12:48:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 14 Sep 2022 12:48:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 14 Sep 2022 12:48:52 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 14 Sep 2022 12:49:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 14 Sep 2022 12:49:30 GMT
ENV GOPATH=C:\go
# Wed, 14 Sep 2022 12:49:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 04 Oct 2022 19:40:59 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:44:14 GMT
RUN $url = 'https://dl.google.com/go/go1.19.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e132d4f0518b0d417eb6cc5f182c3385f6d24bb2eebee2566cd1a7ab6097e3f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 04 Oct 2022 19:44:16 GMT
WORKDIR C:\go
# Tue, 04 Oct 2022 20:37:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 04 Oct 2022 20:37:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:37:19 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:37:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:37:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 04 Oct 2022 20:37:54 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6316baacdbe5997d732fa3555c0cd6f52fd467b41d4d41b596d460cfe8aa`  
		Last Modified: Wed, 14 Sep 2022 13:23:35 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de847c6f89452694f7278d29e3920062ee79faf74467742e329a71dc1db8805`  
		Last Modified: Wed, 14 Sep 2022 13:23:32 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1a6aca4358241a5ae1012bcd11240db54df9849aa25d07166c302dd3014dee`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a0740ce986dad4039bc222ec6cfe798adfe4573d313d4e3583b8694109298e`  
		Last Modified: Wed, 14 Sep 2022 13:23:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ed2e7f7ad8700539fdcbbfa0a73ce470c9b68aad955ee06135135e35f19d3`  
		Last Modified: Wed, 14 Sep 2022 13:23:39 GMT  
		Size: 25.7 MB (25676400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde228a76aaef32add4bb50c16be55584a1328125aa2b2436d22da9d311837a4`  
		Last Modified: Wed, 14 Sep 2022 13:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab59b5ad3cb6d91ad9c3a3064155bffbd0cafff4fa66dc0d04e68d873a23c2c9`  
		Last Modified: Wed, 14 Sep 2022 13:23:29 GMT  
		Size: 526.6 KB (526562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7b60da979d12d87db1ff1c51bfbdabdf15744a9fc23c48d1f527d0d64a525`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915d3981a43f92982ff6e6db42d677c0a5c719a6956d8a7fc5fdcbf22a69837e`  
		Last Modified: Tue, 04 Oct 2022 20:13:30 GMT  
		Size: 157.8 MB (157822684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80571c0669f0277abd15b39422c7ac33098824b4e3acd5165a1094baff1c24a0`  
		Last Modified: Tue, 04 Oct 2022 20:12:49 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce18cf0a5122414eb1417b6ea89e2af5dcbcfe8c8122f793c70530b5dfe185`  
		Last Modified: Tue, 04 Oct 2022 20:38:56 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6550656e761fb3dd33274b46efce609cf133d7ed5c3d2225307cb86e915686`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa241376abdf364b18ef913f22cd27f760430d56204f746263e788237ad2bc7b`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b0bbe614d6c4745bef5fb8c12ed68f7b5098aba644c3702b2c751772ff8dca`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83010d61e0e222aba800d09aa0e6f101273aa57850a02045c234cf45a46c26a`  
		Last Modified: Tue, 04 Oct 2022 20:38:54 GMT  
		Size: 1.8 MB (1834812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cece43f8685aa24f6224e5c09637d5766d50638f619e13f1ea4f6f5a6797992`  
		Last Modified: Tue, 04 Oct 2022 20:38:53 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:3f766f2dc97b6440bb6dcc8f105279999c60d6e0382403d7ab3be51329a692cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:5e68e231a2fb583cc2bafe472844495cd9c1b119b626cb61777a75f990886906
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181f13e1cc5fd90d0b4869e57689b5200589ca1029971fc7233082c04806a55b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 04:34:57 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 04:34:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 04:34:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 04:35:00 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 04:35:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 04:35:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 04:35:01 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 04:35:01 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 04:35:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890b94b17a6b1f257ddec10a103ff342db99516b0d339260623d6610db9b1349`  
		Last Modified: Fri, 07 Oct 2022 04:35:27 GMT  
		Size: 14.5 MB (14493818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d852ea4bd9f60570e83e432bcb361e0400dc3b2c3a264a447dfc2f6b292c0a`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:12eface0625a91f60ec1e6f8ccd864d52c9dc69f3b02ea126e4fdaacf8de5bd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0d4211357adf7a3124613f982947e3745803a9205db56b524ae70f1f03f521`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 04:09:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 08 Oct 2022 04:09:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Sat, 08 Oct 2022 04:09:55 GMT
ENV CADDY_VERSION=v2.6.1
# Sat, 08 Oct 2022 04:09:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 08 Oct 2022 04:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 08 Oct 2022 04:09:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 08 Oct 2022 04:09:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 80
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443
# Sat, 08 Oct 2022 04:09:59 GMT
EXPOSE 443/udp
# Sat, 08 Oct 2022 04:10:00 GMT
EXPOSE 2019
# Sat, 08 Oct 2022 04:10:00 GMT
WORKDIR /srv
# Sat, 08 Oct 2022 04:10:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa0e79d89709c451dcc1ed2799b94c19204fb58ea7cce7895eef1f51c01bb50`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 304.5 KB (304488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9215626c7fc1bfbffb15114b3a5de7fc64de1e7a2a21ee2056121f5ef65b2338`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ca8b546a2bb8c3467ac3eafdca5479dd6396e518b348315a1b16a18519b61`  
		Last Modified: Sat, 08 Oct 2022 04:10:49 GMT  
		Size: 13.8 MB (13848654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e20fa1676a89097bb7bfd9deb83ec1b2ba35972a2c365e7e0b111bf46a430`  
		Last Modified: Sat, 08 Oct 2022 04:10:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:8c5c01339078f89f85a5a7cd08d8bd89962900d295af83cc0eb70de31c4d51ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c275d9a5ca87dde16a12a6d524b9a542b9e77e96ead14f8c577857b6091f24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:17:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:17:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:17:46 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:17:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:17:50 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:17:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:17:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:17:51 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:17:52 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:17:52 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:17:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11d99bb68cba432782c86e461f4c830d8bc08ba0b2df2999db3ab67a55f57e`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 303.6 KB (303619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30dd3a0b20a2d25c12f53bf9ae92037f177e924b7613dbbeedca0029d44215`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf0645b8aab72e227505345e7745508a1f23ed2ff304884458f31d828eac843`  
		Last Modified: Fri, 07 Oct 2022 07:18:46 GMT  
		Size: 13.8 MB (13824551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978d7d8e43141c7a175739d7aafcb64b5b8f6561efb3295d91c186bfab20eb3`  
		Last Modified: Fri, 07 Oct 2022 07:18:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e6d1ad533fd36cd36a387471e708740876c809760795f8868490beab7d98443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1814d3a7f6c971e84b565c46272fc51961c9e67e0e8787781be733c087a22`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 08:00:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 08:00:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 08:00:59 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 08:01:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 08:01:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 08:01:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 08:01:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 08:01:06 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 08:01:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 08:01:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 08:01:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 08:01:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 08:01:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 08:01:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 08:01:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 08:01:14 GMT
EXPOSE 80
# Fri, 07 Oct 2022 08:01:15 GMT
EXPOSE 443
# Fri, 07 Oct 2022 08:01:16 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 08:01:17 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 08:01:18 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 08:01:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6fca9d7511cb60edf3b5df387d6b1fd5aaac17867575fc733cf40137b95a90`  
		Last Modified: Fri, 07 Oct 2022 08:02:04 GMT  
		Size: 304.3 KB (304303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8483ebae1fd52b4e5a413ddd322fedfc3978bd5f95dfd62ea2c53f1a0b7a7e05`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 5.8 KB (5755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ad12dc08ecd5447289e06895740be336d526d7bec274b5cab707b3be6c4df`  
		Last Modified: Fri, 07 Oct 2022 08:02:05 GMT  
		Size: 13.2 MB (13196260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b783a84a1d985b8c4d150880a665dffed5e8d3cd282ed0f45af0b28e45c30a`  
		Last Modified: Fri, 07 Oct 2022 08:02:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:3c296624df3a6ffb31e3a5eca10b509c80150fe12e9b19ebf27e061189d44278
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4250b6ab2344a47d567b072f8080c8f6aa93b04bd773b51fa57148ac08e30379`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 07:56:13 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 07:56:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 07:56:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 07:56:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 07:56:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 07:56:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 07:56:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:56:21 GMT
EXPOSE 443
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 07:56:22 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 07:56:22 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 07:56:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d070e557e928b65136b4bb037dd73ddfb5be784310db1f0f3640ce1216afc`  
		Last Modified: Fri, 07 Oct 2022 07:57:11 GMT  
		Size: 12.9 MB (12853693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40adebe65a7cbe002c94177299a2ae8a216f554d7d6ae5eec0916ba7330da421`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:3e5aa9861d4d5e9c0dfda105fa0b598ee20d5f254b734f5a418c99f6a5b9b5af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2a3441daa59cefaa1dbb6d0edd094f53abe4b3c89877fd3b7121dd53d15ef3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 07 Oct 2022 10:23:51 GMT
ENV CADDY_VERSION=v2.6.1
# Fri, 07 Oct 2022 10:23:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 07 Oct 2022 10:24:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 07 Oct 2022 10:24:03 GMT
ENV XDG_DATA_HOME=/data
# Fri, 07 Oct 2022 10:24:04 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Fri, 07 Oct 2022 10:24:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 07 Oct 2022 10:24:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 07 Oct 2022 10:24:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 07 Oct 2022 10:24:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 07 Oct 2022 10:24:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 07 Oct 2022 10:24:09 GMT
EXPOSE 80
# Fri, 07 Oct 2022 10:24:10 GMT
EXPOSE 443
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 443/udp
# Fri, 07 Oct 2022 10:24:11 GMT
EXPOSE 2019
# Fri, 07 Oct 2022 10:24:12 GMT
WORKDIR /srv
# Fri, 07 Oct 2022 10:24:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8c37b8106cb4218c6396b95deabef48406b60274cd3304a53e50b645cd9e7`  
		Last Modified: Fri, 07 Oct 2022 10:25:13 GMT  
		Size: 14.0 MB (14001566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334954d04c67d43f4bab0b7774053bae33c535a25cc073cf20528174bf6031e9`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:a2f4650d657ce94148fda7db712cc27b1cf037cd53535cdcfe6021488cb35680
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3406; amd64
	-	windows version 10.0.20348.1006; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:f65a2a6e954346897215a9d2fa42d57afe06720d80aa6f5ee846aea9dd2343e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:bdc4ef35d7883964347cd421d0c7f4d1204dd4ba43c6fe0e69507caa08592751
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9773ea78bb70d9662b92357e3b85c736d09eebd4a1e8a9f6bd385e0566c999`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:56:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:14:50 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:16:03 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:16:04 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:16:05 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:12 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:13 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:14 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:15 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:17:02 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:17:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960fd8e6814d787fc5e265195b663de23b9c3c3b12c6cc81f04bc52c66047452`  
		Last Modified: Wed, 14 Sep 2022 18:04:54 GMT  
		Size: 359.9 KB (359924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816febcb1a38b5d1af4f6dee36663e9877cdac01c80850f842b35d9caecf92ae`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa28fe41243765918f567f58a49b8ebe3301e4d34d333312651baf98d6e72`  
		Last Modified: Thu, 22 Sep 2022 19:21:03 GMT  
		Size: 14.9 MB (14903503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b3e31f99ec6db7d6a3afb3158886428320e6cd7ebf66cc2863d6783f4e485e`  
		Last Modified: Thu, 22 Sep 2022 19:21:00 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7100a2f393cb15139abf619d5e4ae63bc7d542a34ab645d96d2492b66d038fc2`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96626f97d473234bbc2d5b9dc9bc668fc55962f693ae055d924bfa62e5a5f1`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ba814ad9c87b0ab8d4135ddb02a923814641db5d082bab11caf21cc0c58d69`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b390b87a1bcb0ee2d3375c4be6463cadc215a55518f373b5f433c18b16846b`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a6b1c9e1bfce85927f0652af1a806db00d3fe247473a199a79e4262b833a8`  
		Last Modified: Thu, 22 Sep 2022 19:20:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f6c551e4f2114189ca817eeefd0547a4305a17c53321734e2c34eda0a5d6ab`  
		Last Modified: Thu, 22 Sep 2022 19:20:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0438f6c8e7128eae37f6d187df365c0b10ae971130c920a19e3b545d0dc9bec2`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169962f58de213bc2e53352c2dd01d3be7216994c71da26bbf1abd1f78d3200`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455b4ff109b96370ef48bb80c51ed5f830576fda5313ca6fcde0a5361eee32e9`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db5be8ae427bcc2fb8f461d11bc0ef62407e758e75cd00d4ea824b710e08b1`  
		Last Modified: Thu, 22 Sep 2022 19:20:55 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162cd16e4b63509a43234902113f1f7a53b8991e8f0ff3fe22bde5dc62aaa4bd`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e27a1ef30f83d2480374f77c7c87254eae01b996408927858e9ebd9a1cd119`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644f884504146da3468d6207a0ec0c8ee671239f2064e3c83637087004c5e9f`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81edb5dfd735e10c850d2c9c4255c5c6530c56aafe6a627ff6e0bcfb38e3cf0`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 308.1 KB (308108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d2825454238ef7d4f8e6fce7353d1678ae02fe14be8700a7bad74b5c584573`  
		Last Modified: Thu, 22 Sep 2022 19:20:53 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:391c3e9d6a79f66b9cfdc3800ac89da113665ef28bd627bc2ae077a8fdffa0d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:98d1ea6c9bd3477d53058cc223d7df639cefe9cdd00732156de3efb89c02bdc3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17916af6760a48fdf2ac93f39ba1cb7946463c0dc04f700068512ed52c8cb93e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:59:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 22 Sep 2022 19:17:18 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:17:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e936569b6cec59693a7b588d88c7cffd71bdf2c411e8d1e120f2d8b16db04ff25041e3f747f27c750c045440f5a738ea91aa6ac12be2a1bb85d6ffdd2d8c351f')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 22 Sep 2022 19:17:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 22 Sep 2022 19:17:51 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:17:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:17:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:17:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:17:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:17:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:17:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:17:58 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:17:59 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:18:00 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:18:01 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:18:16 GMT
RUN caddy version
# Thu, 22 Sep 2022 19:18:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282bfce141dcaaa082b6096b4e687653a5dd51f412010dcdb951110bb2614dd`  
		Last Modified: Wed, 14 Sep 2022 18:05:13 GMT  
		Size: 599.8 KB (599836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d297fbae6815106315682db33f0764521572ce4a6643fc4a3ce25fe2ac7ff4`  
		Last Modified: Thu, 22 Sep 2022 19:21:25 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bbb3de6b0bfe565be7d393a88dce48e7c34b0ecf62203e2496282403703507`  
		Last Modified: Thu, 22 Sep 2022 19:21:28 GMT  
		Size: 15.1 MB (15098682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d5cebd51359f9ba36ca45c2e3ededbe5e9310a23d6ca5588797f16698e6d8b`  
		Last Modified: Thu, 22 Sep 2022 19:21:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5171f0f07e9257644ed2d5062630ecf68eb7759c4556631f71df702feee60d9a`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c68db00839762580d7069088563a80bc9c25aa791975d2e7572a431fde1b0`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2fdc67412ebb5158689ac952df17b7ded5a70a68e73c89425601207c0127de`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33bff51b0d07ff0f06ec0d466ffa1eded6472d6ff6ca239b2b79829512e369f`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c4108a476daa71ada1b8ba644957459c29a33c28e27a7f07628aa7e482f26`  
		Last Modified: Thu, 22 Sep 2022 19:21:22 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55a08dc07a9366b70e86ecc7d61b1c683ff45fc7c90ff1f5906bae7d980be20`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3140b8439018d63e40c84ecba0051fa53ad7eaf2c7ff688b5dca13fe785810`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677aaf22bd30eb8e6962f7d2a10a0a18679563f99ddb8b9aaa3c7e46439ea3`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6bcfe3f597d41e55fff6b41240f838e94fb238cea0cbbdbcfdf8d3cf456858`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9cc7f63fa4c19e160eff1f4b38c84eb926809bd7989a4aef0334cf18109e15`  
		Last Modified: Thu, 22 Sep 2022 19:21:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a203a11480b7e637a5a69584e0f30901282d8b140061fff1d3df8eba8f106`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7418875d932ee057d0506f957a8fd18a5221cd1a7d50907ea03e5485cd973e5`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a65db39731dd69dfa8bfcac6c95f6431776c4c7d1459b4a7f39794a1335a05`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c1c17a2596a233c3c26651dc07882894eecb1c5ed8f8084c21420750cc31a`  
		Last Modified: Thu, 22 Sep 2022 19:21:18 GMT  
		Size: 332.3 KB (332334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a86aabc2cfcb48d8740e425c02367dbed519f55b4bd84363f9522bdc1db711`  
		Last Modified: Thu, 22 Sep 2022 19:21:17 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
