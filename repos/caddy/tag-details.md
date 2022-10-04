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
$ docker pull caddy@sha256:faadebac07e5c9daaa97adf528801d228c01d706a6755ab0c082acc4702e25de
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
$ docker pull caddy@sha256:c5422fb96d5bf458fc8a8813354de04ef89cdd6750464608c1a79fa516cb3cf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8159c96a82a85a24bdca751327835b2f572ba3db71f048bfd2a99157c4552a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:21:13 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:21:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:21:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:21:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:21:18 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:21:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4205233f1134d23e80cfe1162f65ddc45f5e08ff0e9b0e8e1f567f1df4868e`  
		Last Modified: Thu, 22 Sep 2022 19:21:41 GMT  
		Size: 14.5 MB (14493827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f35320fa0aa0bd407da7446a532e6bb6ff70ffbbb64aba575f0a6e21ccf51ec`  
		Last Modified: Thu, 22 Sep 2022 19:21:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f2137bdd4a839a19e28becbea0f246fc4597f1d94b9160bbab8d33833a94516a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee668f0f22cd21b96db6834820ac6a8bb48c7e2d0692acea4d45c8da330025c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:49:21 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:49:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:49:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:49:25 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:49:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4bd7a61e1d1d31bb0b5d056e1977f00c6f0b8163f84ac2cc68e852646f3dc3`  
		Last Modified: Thu, 22 Sep 2022 18:50:11 GMT  
		Size: 13.8 MB (13848650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073c127573b2fd3ee6b12c32facd1130f8cc0bea38341433a9964b9284cbf7e`  
		Last Modified: Thu, 22 Sep 2022 18:50:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:754a4ef354849e835ad2f064371f199e12d40bd3a80e2762021dbd80fef7c09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd21ed1eea16f7633d2d018d09b22db42d8bb871a5e2766b2035dc2f9bf68a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:57:20 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:57:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:57:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:57:24 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff391a21d5bd9ec72ea8acc2167c33b229a59f8d895b07f936d10a36f933f85c`  
		Last Modified: Thu, 22 Sep 2022 18:58:08 GMT  
		Size: 13.8 MB (13824532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a0ca8c098350a18188ff1d9a504f8f26fa2877de27bf3da050a0b944f8332`  
		Last Modified: Thu, 22 Sep 2022 18:58:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:91ec6f75105a515495f3e158f4ca7330acf40f7853f554551c083988c668d3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fd3ed314bb850c421d68a78109b3a91fefc6042029dbf260b55437858a1226`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:41:41 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:41:48 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:41:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:41:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:41:56 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:41:57 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:41:58 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:41:59 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:42:00 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:42:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173eaf2f5d3a64c1a049b7d37dae2bd5b53c6523dae94e9d5aa27953c5b6f2a`  
		Last Modified: Thu, 22 Sep 2022 19:42:44 GMT  
		Size: 13.2 MB (13196254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa836aafb15eb36353931beffa1076de802cab80de1ac30f53fe21aca65c6768`  
		Last Modified: Thu, 22 Sep 2022 19:42:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:b7f03acd5c95c3455c9ce665785094ab0a08a757428c633d02b38e88204d533b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89193f536932af1c50b869234fb5354966b6af6bae71497c49c9bd2ba58e8d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:16:17 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:16:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:26 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:16:26 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:16:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57cf77fded040254299e259088c60baca34a7b637739623d4ef8b6e1aee8cc`  
		Last Modified: Thu, 22 Sep 2022 19:17:11 GMT  
		Size: 12.9 MB (12853691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060df16a418309fc2e3f0b60e8eec07b0aff8301ea214986b2e52de5ed766b28`  
		Last Modified: Thu, 22 Sep 2022 19:17:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:f0302c1158b1f1012c28e30a9f5f34321025ddf9c1f604f3a329b2014594e3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc35bb304c92287f0aa42f10af772c3fcb2086ccddb60f4329be61f6abc43c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:03:35 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:03:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:03:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:03:42 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:03:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cecf0b1f1e9b6a8368ba9be6a20e436697da448defc79dc55108e9ea5629d5`  
		Last Modified: Thu, 22 Sep 2022 19:04:54 GMT  
		Size: 14.0 MB (14001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139004284fd2d833d52451b088c4156944f30e57982c6f6d2a73afddbd1d8679`  
		Last Modified: Thu, 22 Sep 2022 19:04:48 GMT  
		Size: 155.0 B  
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
$ docker pull caddy@sha256:21dbf9101c1eae0e2228f386eefab509d462710c2da97ba45d61c083f3e74fc1
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
$ docker pull caddy@sha256:c5422fb96d5bf458fc8a8813354de04ef89cdd6750464608c1a79fa516cb3cf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8159c96a82a85a24bdca751327835b2f572ba3db71f048bfd2a99157c4552a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:21:13 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:21:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:21:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:21:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:21:18 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:21:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4205233f1134d23e80cfe1162f65ddc45f5e08ff0e9b0e8e1f567f1df4868e`  
		Last Modified: Thu, 22 Sep 2022 19:21:41 GMT  
		Size: 14.5 MB (14493827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f35320fa0aa0bd407da7446a532e6bb6ff70ffbbb64aba575f0a6e21ccf51ec`  
		Last Modified: Thu, 22 Sep 2022 19:21:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f2137bdd4a839a19e28becbea0f246fc4597f1d94b9160bbab8d33833a94516a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee668f0f22cd21b96db6834820ac6a8bb48c7e2d0692acea4d45c8da330025c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:49:21 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:49:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:49:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:49:25 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:49:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4bd7a61e1d1d31bb0b5d056e1977f00c6f0b8163f84ac2cc68e852646f3dc3`  
		Last Modified: Thu, 22 Sep 2022 18:50:11 GMT  
		Size: 13.8 MB (13848650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073c127573b2fd3ee6b12c32facd1130f8cc0bea38341433a9964b9284cbf7e`  
		Last Modified: Thu, 22 Sep 2022 18:50:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:754a4ef354849e835ad2f064371f199e12d40bd3a80e2762021dbd80fef7c09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd21ed1eea16f7633d2d018d09b22db42d8bb871a5e2766b2035dc2f9bf68a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:57:20 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:57:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:57:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:57:24 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff391a21d5bd9ec72ea8acc2167c33b229a59f8d895b07f936d10a36f933f85c`  
		Last Modified: Thu, 22 Sep 2022 18:58:08 GMT  
		Size: 13.8 MB (13824532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a0ca8c098350a18188ff1d9a504f8f26fa2877de27bf3da050a0b944f8332`  
		Last Modified: Thu, 22 Sep 2022 18:58:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:91ec6f75105a515495f3e158f4ca7330acf40f7853f554551c083988c668d3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fd3ed314bb850c421d68a78109b3a91fefc6042029dbf260b55437858a1226`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:41:41 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:41:48 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:41:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:41:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:41:56 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:41:57 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:41:58 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:41:59 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:42:00 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:42:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173eaf2f5d3a64c1a049b7d37dae2bd5b53c6523dae94e9d5aa27953c5b6f2a`  
		Last Modified: Thu, 22 Sep 2022 19:42:44 GMT  
		Size: 13.2 MB (13196254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa836aafb15eb36353931beffa1076de802cab80de1ac30f53fe21aca65c6768`  
		Last Modified: Thu, 22 Sep 2022 19:42:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b7f03acd5c95c3455c9ce665785094ab0a08a757428c633d02b38e88204d533b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89193f536932af1c50b869234fb5354966b6af6bae71497c49c9bd2ba58e8d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:16:17 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:16:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:26 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:16:26 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:16:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57cf77fded040254299e259088c60baca34a7b637739623d4ef8b6e1aee8cc`  
		Last Modified: Thu, 22 Sep 2022 19:17:11 GMT  
		Size: 12.9 MB (12853691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060df16a418309fc2e3f0b60e8eec07b0aff8301ea214986b2e52de5ed766b28`  
		Last Modified: Thu, 22 Sep 2022 19:17:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f0302c1158b1f1012c28e30a9f5f34321025ddf9c1f604f3a329b2014594e3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc35bb304c92287f0aa42f10af772c3fcb2086ccddb60f4329be61f6abc43c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:03:35 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:03:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:03:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:03:42 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:03:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cecf0b1f1e9b6a8368ba9be6a20e436697da448defc79dc55108e9ea5629d5`  
		Last Modified: Thu, 22 Sep 2022 19:04:54 GMT  
		Size: 14.0 MB (14001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139004284fd2d833d52451b088c4156944f30e57982c6f6d2a73afddbd1d8679`  
		Last Modified: Thu, 22 Sep 2022 19:04:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:7074b59735ddf6643ff6d00f59901a9c46478911fb6f0b8a83218e8a755cd7dc
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
$ docker pull caddy@sha256:806531835a3ee4b98692120ba7d5d77ac9f67511336e958a94e3549835582506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133499962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd36cbedf423aed317a7e06e0972147588fccb7de574399071068df83b945ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:54 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:42:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:42:33 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:42:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:42:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:42:34 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:09:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:09:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:09:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:09:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d81b0672f0319abbe5d231bb316a758f235e12071775381065b3b787f6121`  
		Last Modified: Tue, 04 Oct 2022 19:51:00 GMT  
		Size: 122.3 MB (122251625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277b443bd1a959724dd2b3a89b8e8543f8a7de36f62be65f2126b879ad5c8ad`  
		Last Modified: Tue, 04 Oct 2022 19:50:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c8786f0992e8dd727c0222b7d05611f30c7eca1bbaeda8313d28a5e718b541`  
		Last Modified: Tue, 04 Oct 2022 20:09:36 GMT  
		Size: 6.9 MB (6941670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8144098c5e0f2da20fdee70369ed4ae79b2b710c60dac6da94801fa9c8c1cc`  
		Last Modified: Tue, 04 Oct 2022 20:09:35 GMT  
		Size: 1.2 MB (1215172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfff0203e2ac04ac7edadd406708b3360bfc6bd4ebb109b85827a4eb9f177f8`  
		Last Modified: Tue, 04 Oct 2022 20:09:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f73afa45a85262dc63d4d983ab2da8e0eead8b7760f0039c199e732fca5885ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638a32ec67f67b37f9cb0d65ae80161b7823754208317f3342c25b1d40b5ee3c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:39:35 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:49:16 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:49:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:49:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:49:17 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:30:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:30:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:30:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d349e0f4f9311c744c13786b11824154e1c08216ad948d5ebe82875cb878bd7`  
		Last Modified: Tue, 04 Oct 2022 20:12:32 GMT  
		Size: 118.6 MB (118635919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf625d0f07ffea6400b4db19ae8153464917f23dbf61749929881eeb2b37fb8`  
		Last Modified: Tue, 04 Oct 2022 20:12:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e7fcc5c56e0e9828396fa37456be04a382caec3623869e4e66da9790681e6`  
		Last Modified: Tue, 04 Oct 2022 20:31:23 GMT  
		Size: 6.8 MB (6808221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c653d47fa466da3e7b3a3bd7f075c55ff07045cd227a53eae150d5bdd295c1b`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 1.2 MB (1162979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96ffbe114ba0a9a2f25781826343ada15f29699fd17e821c3afd6dc66b3072`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9c9aa1fce6c5b5cfcd3653fff55bdbbcf2ef34bac0a2e82dc6fe2d7a452fb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0067bb4da6d1523159ac91a84a2efae963acb89737ee757ad59cbcd16937a71f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:51 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 20:02:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 20:02:23 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 20:02:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 20:02:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 20:02:24 GMT
WORKDIR /go
# Tue, 04 Oct 2022 21:25:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 21:25:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 21:25:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 21:25:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371376b3d092072c91d12b8ae8b6d7c23dd222982378385554faee7555afbc9`  
		Last Modified: Tue, 04 Oct 2022 20:21:44 GMT  
		Size: 118.4 MB (118407284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed516331f5140684e05fdce25e0c0295e18775b343abe2bc63e1bb63c421d868`  
		Last Modified: Tue, 04 Oct 2022 20:21:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa31122002e131a4f100cc84e1f6b72b13c4b1f04381ac5498c42f9781284b`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 6.1 MB (6067866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b0b98df7e01c28c9f664ee59268827a69c3c79c171a02b02ffef9228b6f51`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 1.2 MB (1159980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ee7662f86e2b1be0d4fe7186bad48ae5e8ca0139df09176f358d98cb0cf79`  
		Last Modified: Tue, 04 Oct 2022 21:25:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:df36211ea8e22d85aa48a71f47b84e71075e5cd4cff8a7bd56e32d39ac40b9f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127985085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b13b26f783107c940301d0a957e2aee82d9ad5c03d4c4ae555a58842cadfd88`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:54:14 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:55:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:55:51 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:55:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:55:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:55:53 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:23:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:23:07 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:23:08 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:23:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:23:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:23:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:23:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4c96e872d58125e8e270e7f4c23f0001b8b8b8e32cd703fda75a7bd5ea6a63`  
		Last Modified: Tue, 04 Oct 2022 20:04:46 GMT  
		Size: 116.8 MB (116819377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d612e3ed75f66cf36584943357bb01e4c52945cae40319c28839a9d2993ab8`  
		Last Modified: Tue, 04 Oct 2022 20:04:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8636190f09c5dea38074348308fbd34bc62d9cdce351d95d15bea5504394e3b3`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 7.1 MB (7052392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf5d35a9434ec361ff62efef87605c4eedf5e5ba36f33b45e62d98b79700a5c`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 1.1 MB (1120445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a19533d345cf495d46b1b208b6ea2871a911516c987dc33830e8c6dbad4de2`  
		Last Modified: Tue, 04 Oct 2022 20:23:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:dcf7bef383bc2ef1a9c06670f66c301437106cf6024797255490daa02015f496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128881670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfde85aab958fe6830006ee81bca416ae8dcd25d1b9dde9852c1fdc4b3e01b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:18 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:43:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:43:10 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:43:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:43:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:43:11 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:14:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:14:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:14:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:14:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f162d01985672827ddfb048d004dd524a6cf77a6564ccec1a1b2bb1ca70870`  
		Last Modified: Tue, 04 Oct 2022 19:55:34 GMT  
		Size: 117.2 MB (117204653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c83a388b1d0281151c0ad223e2882ab7835560f24ff8632c6b5572bd52017`  
		Last Modified: Tue, 04 Oct 2022 19:55:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8f0ceb0d32500e04e62486c61d02503e801fb4f11e716eee78234b59f10881`  
		Last Modified: Tue, 04 Oct 2022 20:15:00 GMT  
		Size: 7.5 MB (7482404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a10426e8126ad610a88c0c67c544ec6ad934ba8727e6f432800b5ff279cd11`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 1.1 MB (1103844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11669aeca9837785668f17d866c23756bc9c3978df3d5e84476f32565fd2e589`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:404f3025fa1bf713807ae106c84550d7cc438726dc68e06a917dd9a2999bc0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131828807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528fbc52d70c938ac901a877c243b4ddf059ab8e5071d26ed00c4cb598a58a4b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:51:13 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:53:48 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:53:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:53:49 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:24:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:24:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:24:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:24:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1238bfd151683573cd911e00a0ecb201b2a754f39b8a62e7d0cfe908734d31`  
		Last Modified: Tue, 04 Oct 2022 20:06:50 GMT  
		Size: 120.7 MB (120732088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c161868cfaa1386086f2ebfb88351c233b6b6c0db49a37ae9f06fc971270abce`  
		Last Modified: Tue, 04 Oct 2022 20:06:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20be2863c9fe0842a12f57089063e87713658c0acb8656e230a988f99cdefa`  
		Last Modified: Tue, 04 Oct 2022 20:25:07 GMT  
		Size: 7.1 MB (7053038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5842247ede61565ac01c0eccc30149d27e311f6aa7f3a7ad20c56fbb247ffb2`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 1.2 MB (1167425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a54f79a30bd281d6df17484fdc97e05e169cf138a5b2eff5ebb6932bcd26249`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:8106c25f6910ae0302bffc6b16ae6e8a7d9a9a4cd90d3e8007a7856b5c2d82eb
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
$ docker pull caddy@sha256:806531835a3ee4b98692120ba7d5d77ac9f67511336e958a94e3549835582506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133499962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd36cbedf423aed317a7e06e0972147588fccb7de574399071068df83b945ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:54 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:42:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:42:33 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:42:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:42:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:42:34 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:09:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:09:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:09:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:09:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d81b0672f0319abbe5d231bb316a758f235e12071775381065b3b787f6121`  
		Last Modified: Tue, 04 Oct 2022 19:51:00 GMT  
		Size: 122.3 MB (122251625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277b443bd1a959724dd2b3a89b8e8543f8a7de36f62be65f2126b879ad5c8ad`  
		Last Modified: Tue, 04 Oct 2022 19:50:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c8786f0992e8dd727c0222b7d05611f30c7eca1bbaeda8313d28a5e718b541`  
		Last Modified: Tue, 04 Oct 2022 20:09:36 GMT  
		Size: 6.9 MB (6941670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8144098c5e0f2da20fdee70369ed4ae79b2b710c60dac6da94801fa9c8c1cc`  
		Last Modified: Tue, 04 Oct 2022 20:09:35 GMT  
		Size: 1.2 MB (1215172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfff0203e2ac04ac7edadd406708b3360bfc6bd4ebb109b85827a4eb9f177f8`  
		Last Modified: Tue, 04 Oct 2022 20:09:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f73afa45a85262dc63d4d983ab2da8e0eead8b7760f0039c199e732fca5885ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638a32ec67f67b37f9cb0d65ae80161b7823754208317f3342c25b1d40b5ee3c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:39:35 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:49:16 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:49:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:49:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:49:17 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:30:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:30:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:30:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d349e0f4f9311c744c13786b11824154e1c08216ad948d5ebe82875cb878bd7`  
		Last Modified: Tue, 04 Oct 2022 20:12:32 GMT  
		Size: 118.6 MB (118635919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf625d0f07ffea6400b4db19ae8153464917f23dbf61749929881eeb2b37fb8`  
		Last Modified: Tue, 04 Oct 2022 20:12:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e7fcc5c56e0e9828396fa37456be04a382caec3623869e4e66da9790681e6`  
		Last Modified: Tue, 04 Oct 2022 20:31:23 GMT  
		Size: 6.8 MB (6808221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c653d47fa466da3e7b3a3bd7f075c55ff07045cd227a53eae150d5bdd295c1b`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 1.2 MB (1162979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96ffbe114ba0a9a2f25781826343ada15f29699fd17e821c3afd6dc66b3072`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9c9aa1fce6c5b5cfcd3653fff55bdbbcf2ef34bac0a2e82dc6fe2d7a452fb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0067bb4da6d1523159ac91a84a2efae963acb89737ee757ad59cbcd16937a71f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:51 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 20:02:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 20:02:23 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 20:02:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 20:02:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 20:02:24 GMT
WORKDIR /go
# Tue, 04 Oct 2022 21:25:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 21:25:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 21:25:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 21:25:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371376b3d092072c91d12b8ae8b6d7c23dd222982378385554faee7555afbc9`  
		Last Modified: Tue, 04 Oct 2022 20:21:44 GMT  
		Size: 118.4 MB (118407284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed516331f5140684e05fdce25e0c0295e18775b343abe2bc63e1bb63c421d868`  
		Last Modified: Tue, 04 Oct 2022 20:21:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa31122002e131a4f100cc84e1f6b72b13c4b1f04381ac5498c42f9781284b`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 6.1 MB (6067866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b0b98df7e01c28c9f664ee59268827a69c3c79c171a02b02ffef9228b6f51`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 1.2 MB (1159980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ee7662f86e2b1be0d4fe7186bad48ae5e8ca0139df09176f358d98cb0cf79`  
		Last Modified: Tue, 04 Oct 2022 21:25:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:df36211ea8e22d85aa48a71f47b84e71075e5cd4cff8a7bd56e32d39ac40b9f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127985085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b13b26f783107c940301d0a957e2aee82d9ad5c03d4c4ae555a58842cadfd88`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:54:14 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:55:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:55:51 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:55:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:55:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:55:53 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:23:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:23:07 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:23:08 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:23:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:23:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:23:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:23:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4c96e872d58125e8e270e7f4c23f0001b8b8b8e32cd703fda75a7bd5ea6a63`  
		Last Modified: Tue, 04 Oct 2022 20:04:46 GMT  
		Size: 116.8 MB (116819377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d612e3ed75f66cf36584943357bb01e4c52945cae40319c28839a9d2993ab8`  
		Last Modified: Tue, 04 Oct 2022 20:04:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8636190f09c5dea38074348308fbd34bc62d9cdce351d95d15bea5504394e3b3`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 7.1 MB (7052392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf5d35a9434ec361ff62efef87605c4eedf5e5ba36f33b45e62d98b79700a5c`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 1.1 MB (1120445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a19533d345cf495d46b1b208b6ea2871a911516c987dc33830e8c6dbad4de2`  
		Last Modified: Tue, 04 Oct 2022 20:23:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:dcf7bef383bc2ef1a9c06670f66c301437106cf6024797255490daa02015f496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128881670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfde85aab958fe6830006ee81bca416ae8dcd25d1b9dde9852c1fdc4b3e01b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:18 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:43:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:43:10 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:43:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:43:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:43:11 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:14:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:14:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:14:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:14:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f162d01985672827ddfb048d004dd524a6cf77a6564ccec1a1b2bb1ca70870`  
		Last Modified: Tue, 04 Oct 2022 19:55:34 GMT  
		Size: 117.2 MB (117204653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c83a388b1d0281151c0ad223e2882ab7835560f24ff8632c6b5572bd52017`  
		Last Modified: Tue, 04 Oct 2022 19:55:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8f0ceb0d32500e04e62486c61d02503e801fb4f11e716eee78234b59f10881`  
		Last Modified: Tue, 04 Oct 2022 20:15:00 GMT  
		Size: 7.5 MB (7482404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a10426e8126ad610a88c0c67c544ec6ad934ba8727e6f432800b5ff279cd11`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 1.1 MB (1103844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11669aeca9837785668f17d866c23756bc9c3978df3d5e84476f32565fd2e589`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:404f3025fa1bf713807ae106c84550d7cc438726dc68e06a917dd9a2999bc0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131828807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528fbc52d70c938ac901a877c243b4ddf059ab8e5071d26ed00c4cb598a58a4b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:51:13 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:53:48 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:53:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:53:49 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:24:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:24:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:24:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:24:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1238bfd151683573cd911e00a0ecb201b2a754f39b8a62e7d0cfe908734d31`  
		Last Modified: Tue, 04 Oct 2022 20:06:50 GMT  
		Size: 120.7 MB (120732088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c161868cfaa1386086f2ebfb88351c233b6b6c0db49a37ae9f06fc971270abce`  
		Last Modified: Tue, 04 Oct 2022 20:06:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20be2863c9fe0842a12f57089063e87713658c0acb8656e230a988f99cdefa`  
		Last Modified: Tue, 04 Oct 2022 20:25:07 GMT  
		Size: 7.1 MB (7053038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5842247ede61565ac01c0eccc30149d27e311f6aa7f3a7ad20c56fbb247ffb2`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 1.2 MB (1167425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a54f79a30bd281d6df17484fdc97e05e169cf138a5b2eff5ebb6932bcd26249`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:faadebac07e5c9daaa97adf528801d228c01d706a6755ab0c082acc4702e25de
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
$ docker pull caddy@sha256:c5422fb96d5bf458fc8a8813354de04ef89cdd6750464608c1a79fa516cb3cf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8159c96a82a85a24bdca751327835b2f572ba3db71f048bfd2a99157c4552a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:21:13 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:21:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:21:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:21:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:21:18 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:21:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4205233f1134d23e80cfe1162f65ddc45f5e08ff0e9b0e8e1f567f1df4868e`  
		Last Modified: Thu, 22 Sep 2022 19:21:41 GMT  
		Size: 14.5 MB (14493827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f35320fa0aa0bd407da7446a532e6bb6ff70ffbbb64aba575f0a6e21ccf51ec`  
		Last Modified: Thu, 22 Sep 2022 19:21:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f2137bdd4a839a19e28becbea0f246fc4597f1d94b9160bbab8d33833a94516a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee668f0f22cd21b96db6834820ac6a8bb48c7e2d0692acea4d45c8da330025c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:49:21 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:49:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:49:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:49:25 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:49:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4bd7a61e1d1d31bb0b5d056e1977f00c6f0b8163f84ac2cc68e852646f3dc3`  
		Last Modified: Thu, 22 Sep 2022 18:50:11 GMT  
		Size: 13.8 MB (13848650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073c127573b2fd3ee6b12c32facd1130f8cc0bea38341433a9964b9284cbf7e`  
		Last Modified: Thu, 22 Sep 2022 18:50:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:754a4ef354849e835ad2f064371f199e12d40bd3a80e2762021dbd80fef7c09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd21ed1eea16f7633d2d018d09b22db42d8bb871a5e2766b2035dc2f9bf68a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:57:20 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:57:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:57:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:57:24 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff391a21d5bd9ec72ea8acc2167c33b229a59f8d895b07f936d10a36f933f85c`  
		Last Modified: Thu, 22 Sep 2022 18:58:08 GMT  
		Size: 13.8 MB (13824532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a0ca8c098350a18188ff1d9a504f8f26fa2877de27bf3da050a0b944f8332`  
		Last Modified: Thu, 22 Sep 2022 18:58:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:91ec6f75105a515495f3e158f4ca7330acf40f7853f554551c083988c668d3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fd3ed314bb850c421d68a78109b3a91fefc6042029dbf260b55437858a1226`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:41:41 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:41:48 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:41:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:41:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:41:56 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:41:57 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:41:58 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:41:59 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:42:00 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:42:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173eaf2f5d3a64c1a049b7d37dae2bd5b53c6523dae94e9d5aa27953c5b6f2a`  
		Last Modified: Thu, 22 Sep 2022 19:42:44 GMT  
		Size: 13.2 MB (13196254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa836aafb15eb36353931beffa1076de802cab80de1ac30f53fe21aca65c6768`  
		Last Modified: Thu, 22 Sep 2022 19:42:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:b7f03acd5c95c3455c9ce665785094ab0a08a757428c633d02b38e88204d533b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89193f536932af1c50b869234fb5354966b6af6bae71497c49c9bd2ba58e8d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:16:17 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:16:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:26 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:16:26 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:16:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57cf77fded040254299e259088c60baca34a7b637739623d4ef8b6e1aee8cc`  
		Last Modified: Thu, 22 Sep 2022 19:17:11 GMT  
		Size: 12.9 MB (12853691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060df16a418309fc2e3f0b60e8eec07b0aff8301ea214986b2e52de5ed766b28`  
		Last Modified: Thu, 22 Sep 2022 19:17:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1` - linux; s390x

```console
$ docker pull caddy@sha256:f0302c1158b1f1012c28e30a9f5f34321025ddf9c1f604f3a329b2014594e3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc35bb304c92287f0aa42f10af772c3fcb2086ccddb60f4329be61f6abc43c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:03:35 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:03:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:03:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:03:42 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:03:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cecf0b1f1e9b6a8368ba9be6a20e436697da448defc79dc55108e9ea5629d5`  
		Last Modified: Thu, 22 Sep 2022 19:04:54 GMT  
		Size: 14.0 MB (14001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139004284fd2d833d52451b088c4156944f30e57982c6f6d2a73afddbd1d8679`  
		Last Modified: Thu, 22 Sep 2022 19:04:48 GMT  
		Size: 155.0 B  
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
$ docker pull caddy@sha256:21dbf9101c1eae0e2228f386eefab509d462710c2da97ba45d61c083f3e74fc1
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
$ docker pull caddy@sha256:c5422fb96d5bf458fc8a8813354de04ef89cdd6750464608c1a79fa516cb3cf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8159c96a82a85a24bdca751327835b2f572ba3db71f048bfd2a99157c4552a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:21:13 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:21:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:21:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:21:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:21:18 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:21:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4205233f1134d23e80cfe1162f65ddc45f5e08ff0e9b0e8e1f567f1df4868e`  
		Last Modified: Thu, 22 Sep 2022 19:21:41 GMT  
		Size: 14.5 MB (14493827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f35320fa0aa0bd407da7446a532e6bb6ff70ffbbb64aba575f0a6e21ccf51ec`  
		Last Modified: Thu, 22 Sep 2022 19:21:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f2137bdd4a839a19e28becbea0f246fc4597f1d94b9160bbab8d33833a94516a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee668f0f22cd21b96db6834820ac6a8bb48c7e2d0692acea4d45c8da330025c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:49:21 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:49:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:49:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:49:25 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:49:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4bd7a61e1d1d31bb0b5d056e1977f00c6f0b8163f84ac2cc68e852646f3dc3`  
		Last Modified: Thu, 22 Sep 2022 18:50:11 GMT  
		Size: 13.8 MB (13848650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073c127573b2fd3ee6b12c32facd1130f8cc0bea38341433a9964b9284cbf7e`  
		Last Modified: Thu, 22 Sep 2022 18:50:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:754a4ef354849e835ad2f064371f199e12d40bd3a80e2762021dbd80fef7c09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd21ed1eea16f7633d2d018d09b22db42d8bb871a5e2766b2035dc2f9bf68a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:57:20 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:57:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:57:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:57:24 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff391a21d5bd9ec72ea8acc2167c33b229a59f8d895b07f936d10a36f933f85c`  
		Last Modified: Thu, 22 Sep 2022 18:58:08 GMT  
		Size: 13.8 MB (13824532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a0ca8c098350a18188ff1d9a504f8f26fa2877de27bf3da050a0b944f8332`  
		Last Modified: Thu, 22 Sep 2022 18:58:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:91ec6f75105a515495f3e158f4ca7330acf40f7853f554551c083988c668d3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fd3ed314bb850c421d68a78109b3a91fefc6042029dbf260b55437858a1226`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:41:41 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:41:48 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:41:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:41:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:41:56 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:41:57 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:41:58 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:41:59 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:42:00 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:42:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173eaf2f5d3a64c1a049b7d37dae2bd5b53c6523dae94e9d5aa27953c5b6f2a`  
		Last Modified: Thu, 22 Sep 2022 19:42:44 GMT  
		Size: 13.2 MB (13196254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa836aafb15eb36353931beffa1076de802cab80de1ac30f53fe21aca65c6768`  
		Last Modified: Thu, 22 Sep 2022 19:42:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b7f03acd5c95c3455c9ce665785094ab0a08a757428c633d02b38e88204d533b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89193f536932af1c50b869234fb5354966b6af6bae71497c49c9bd2ba58e8d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:16:17 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:16:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:26 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:16:26 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:16:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57cf77fded040254299e259088c60baca34a7b637739623d4ef8b6e1aee8cc`  
		Last Modified: Thu, 22 Sep 2022 19:17:11 GMT  
		Size: 12.9 MB (12853691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060df16a418309fc2e3f0b60e8eec07b0aff8301ea214986b2e52de5ed766b28`  
		Last Modified: Thu, 22 Sep 2022 19:17:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f0302c1158b1f1012c28e30a9f5f34321025ddf9c1f604f3a329b2014594e3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc35bb304c92287f0aa42f10af772c3fcb2086ccddb60f4329be61f6abc43c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:03:35 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:03:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:03:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:03:42 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:03:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cecf0b1f1e9b6a8368ba9be6a20e436697da448defc79dc55108e9ea5629d5`  
		Last Modified: Thu, 22 Sep 2022 19:04:54 GMT  
		Size: 14.0 MB (14001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139004284fd2d833d52451b088c4156944f30e57982c6f6d2a73afddbd1d8679`  
		Last Modified: Thu, 22 Sep 2022 19:04:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.1-builder`

```console
$ docker pull caddy@sha256:7074b59735ddf6643ff6d00f59901a9c46478911fb6f0b8a83218e8a755cd7dc
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
$ docker pull caddy@sha256:806531835a3ee4b98692120ba7d5d77ac9f67511336e958a94e3549835582506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133499962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd36cbedf423aed317a7e06e0972147588fccb7de574399071068df83b945ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:54 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:42:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:42:33 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:42:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:42:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:42:34 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:09:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:09:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:09:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:09:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d81b0672f0319abbe5d231bb316a758f235e12071775381065b3b787f6121`  
		Last Modified: Tue, 04 Oct 2022 19:51:00 GMT  
		Size: 122.3 MB (122251625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277b443bd1a959724dd2b3a89b8e8543f8a7de36f62be65f2126b879ad5c8ad`  
		Last Modified: Tue, 04 Oct 2022 19:50:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c8786f0992e8dd727c0222b7d05611f30c7eca1bbaeda8313d28a5e718b541`  
		Last Modified: Tue, 04 Oct 2022 20:09:36 GMT  
		Size: 6.9 MB (6941670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8144098c5e0f2da20fdee70369ed4ae79b2b710c60dac6da94801fa9c8c1cc`  
		Last Modified: Tue, 04 Oct 2022 20:09:35 GMT  
		Size: 1.2 MB (1215172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfff0203e2ac04ac7edadd406708b3360bfc6bd4ebb109b85827a4eb9f177f8`  
		Last Modified: Tue, 04 Oct 2022 20:09:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f73afa45a85262dc63d4d983ab2da8e0eead8b7760f0039c199e732fca5885ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638a32ec67f67b37f9cb0d65ae80161b7823754208317f3342c25b1d40b5ee3c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:39:35 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:49:16 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:49:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:49:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:49:17 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:30:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:30:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:30:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d349e0f4f9311c744c13786b11824154e1c08216ad948d5ebe82875cb878bd7`  
		Last Modified: Tue, 04 Oct 2022 20:12:32 GMT  
		Size: 118.6 MB (118635919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf625d0f07ffea6400b4db19ae8153464917f23dbf61749929881eeb2b37fb8`  
		Last Modified: Tue, 04 Oct 2022 20:12:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e7fcc5c56e0e9828396fa37456be04a382caec3623869e4e66da9790681e6`  
		Last Modified: Tue, 04 Oct 2022 20:31:23 GMT  
		Size: 6.8 MB (6808221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c653d47fa466da3e7b3a3bd7f075c55ff07045cd227a53eae150d5bdd295c1b`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 1.2 MB (1162979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96ffbe114ba0a9a2f25781826343ada15f29699fd17e821c3afd6dc66b3072`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9c9aa1fce6c5b5cfcd3653fff55bdbbcf2ef34bac0a2e82dc6fe2d7a452fb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0067bb4da6d1523159ac91a84a2efae963acb89737ee757ad59cbcd16937a71f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:51 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 20:02:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 20:02:23 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 20:02:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 20:02:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 20:02:24 GMT
WORKDIR /go
# Tue, 04 Oct 2022 21:25:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 21:25:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 21:25:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 21:25:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371376b3d092072c91d12b8ae8b6d7c23dd222982378385554faee7555afbc9`  
		Last Modified: Tue, 04 Oct 2022 20:21:44 GMT  
		Size: 118.4 MB (118407284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed516331f5140684e05fdce25e0c0295e18775b343abe2bc63e1bb63c421d868`  
		Last Modified: Tue, 04 Oct 2022 20:21:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa31122002e131a4f100cc84e1f6b72b13c4b1f04381ac5498c42f9781284b`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 6.1 MB (6067866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b0b98df7e01c28c9f664ee59268827a69c3c79c171a02b02ffef9228b6f51`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 1.2 MB (1159980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ee7662f86e2b1be0d4fe7186bad48ae5e8ca0139df09176f358d98cb0cf79`  
		Last Modified: Tue, 04 Oct 2022 21:25:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:df36211ea8e22d85aa48a71f47b84e71075e5cd4cff8a7bd56e32d39ac40b9f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127985085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b13b26f783107c940301d0a957e2aee82d9ad5c03d4c4ae555a58842cadfd88`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:54:14 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:55:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:55:51 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:55:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:55:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:55:53 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:23:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:23:07 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:23:08 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:23:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:23:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:23:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:23:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4c96e872d58125e8e270e7f4c23f0001b8b8b8e32cd703fda75a7bd5ea6a63`  
		Last Modified: Tue, 04 Oct 2022 20:04:46 GMT  
		Size: 116.8 MB (116819377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d612e3ed75f66cf36584943357bb01e4c52945cae40319c28839a9d2993ab8`  
		Last Modified: Tue, 04 Oct 2022 20:04:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8636190f09c5dea38074348308fbd34bc62d9cdce351d95d15bea5504394e3b3`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 7.1 MB (7052392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf5d35a9434ec361ff62efef87605c4eedf5e5ba36f33b45e62d98b79700a5c`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 1.1 MB (1120445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a19533d345cf495d46b1b208b6ea2871a911516c987dc33830e8c6dbad4de2`  
		Last Modified: Tue, 04 Oct 2022 20:23:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:dcf7bef383bc2ef1a9c06670f66c301437106cf6024797255490daa02015f496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128881670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfde85aab958fe6830006ee81bca416ae8dcd25d1b9dde9852c1fdc4b3e01b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:18 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:43:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:43:10 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:43:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:43:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:43:11 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:14:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:14:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:14:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:14:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f162d01985672827ddfb048d004dd524a6cf77a6564ccec1a1b2bb1ca70870`  
		Last Modified: Tue, 04 Oct 2022 19:55:34 GMT  
		Size: 117.2 MB (117204653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c83a388b1d0281151c0ad223e2882ab7835560f24ff8632c6b5572bd52017`  
		Last Modified: Tue, 04 Oct 2022 19:55:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8f0ceb0d32500e04e62486c61d02503e801fb4f11e716eee78234b59f10881`  
		Last Modified: Tue, 04 Oct 2022 20:15:00 GMT  
		Size: 7.5 MB (7482404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a10426e8126ad610a88c0c67c544ec6ad934ba8727e6f432800b5ff279cd11`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 1.1 MB (1103844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11669aeca9837785668f17d866c23756bc9c3978df3d5e84476f32565fd2e589`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:404f3025fa1bf713807ae106c84550d7cc438726dc68e06a917dd9a2999bc0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131828807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528fbc52d70c938ac901a877c243b4ddf059ab8e5071d26ed00c4cb598a58a4b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:51:13 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:53:48 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:53:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:53:49 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:24:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:24:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:24:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:24:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1238bfd151683573cd911e00a0ecb201b2a754f39b8a62e7d0cfe908734d31`  
		Last Modified: Tue, 04 Oct 2022 20:06:50 GMT  
		Size: 120.7 MB (120732088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c161868cfaa1386086f2ebfb88351c233b6b6c0db49a37ae9f06fc971270abce`  
		Last Modified: Tue, 04 Oct 2022 20:06:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20be2863c9fe0842a12f57089063e87713658c0acb8656e230a988f99cdefa`  
		Last Modified: Tue, 04 Oct 2022 20:25:07 GMT  
		Size: 7.1 MB (7053038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5842247ede61565ac01c0eccc30149d27e311f6aa7f3a7ad20c56fbb247ffb2`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 1.2 MB (1167425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a54f79a30bd281d6df17484fdc97e05e169cf138a5b2eff5ebb6932bcd26249`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:8106c25f6910ae0302bffc6b16ae6e8a7d9a9a4cd90d3e8007a7856b5c2d82eb
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
$ docker pull caddy@sha256:806531835a3ee4b98692120ba7d5d77ac9f67511336e958a94e3549835582506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133499962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd36cbedf423aed317a7e06e0972147588fccb7de574399071068df83b945ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:54 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:42:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:42:33 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:42:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:42:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:42:34 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:09:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:09:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:09:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:09:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d81b0672f0319abbe5d231bb316a758f235e12071775381065b3b787f6121`  
		Last Modified: Tue, 04 Oct 2022 19:51:00 GMT  
		Size: 122.3 MB (122251625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277b443bd1a959724dd2b3a89b8e8543f8a7de36f62be65f2126b879ad5c8ad`  
		Last Modified: Tue, 04 Oct 2022 19:50:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c8786f0992e8dd727c0222b7d05611f30c7eca1bbaeda8313d28a5e718b541`  
		Last Modified: Tue, 04 Oct 2022 20:09:36 GMT  
		Size: 6.9 MB (6941670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8144098c5e0f2da20fdee70369ed4ae79b2b710c60dac6da94801fa9c8c1cc`  
		Last Modified: Tue, 04 Oct 2022 20:09:35 GMT  
		Size: 1.2 MB (1215172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfff0203e2ac04ac7edadd406708b3360bfc6bd4ebb109b85827a4eb9f177f8`  
		Last Modified: Tue, 04 Oct 2022 20:09:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f73afa45a85262dc63d4d983ab2da8e0eead8b7760f0039c199e732fca5885ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638a32ec67f67b37f9cb0d65ae80161b7823754208317f3342c25b1d40b5ee3c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:39:35 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:49:16 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:49:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:49:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:49:17 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:30:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:30:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:30:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d349e0f4f9311c744c13786b11824154e1c08216ad948d5ebe82875cb878bd7`  
		Last Modified: Tue, 04 Oct 2022 20:12:32 GMT  
		Size: 118.6 MB (118635919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf625d0f07ffea6400b4db19ae8153464917f23dbf61749929881eeb2b37fb8`  
		Last Modified: Tue, 04 Oct 2022 20:12:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e7fcc5c56e0e9828396fa37456be04a382caec3623869e4e66da9790681e6`  
		Last Modified: Tue, 04 Oct 2022 20:31:23 GMT  
		Size: 6.8 MB (6808221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c653d47fa466da3e7b3a3bd7f075c55ff07045cd227a53eae150d5bdd295c1b`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 1.2 MB (1162979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96ffbe114ba0a9a2f25781826343ada15f29699fd17e821c3afd6dc66b3072`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9c9aa1fce6c5b5cfcd3653fff55bdbbcf2ef34bac0a2e82dc6fe2d7a452fb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0067bb4da6d1523159ac91a84a2efae963acb89737ee757ad59cbcd16937a71f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:51 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 20:02:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 20:02:23 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 20:02:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 20:02:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 20:02:24 GMT
WORKDIR /go
# Tue, 04 Oct 2022 21:25:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 21:25:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 21:25:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 21:25:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371376b3d092072c91d12b8ae8b6d7c23dd222982378385554faee7555afbc9`  
		Last Modified: Tue, 04 Oct 2022 20:21:44 GMT  
		Size: 118.4 MB (118407284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed516331f5140684e05fdce25e0c0295e18775b343abe2bc63e1bb63c421d868`  
		Last Modified: Tue, 04 Oct 2022 20:21:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa31122002e131a4f100cc84e1f6b72b13c4b1f04381ac5498c42f9781284b`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 6.1 MB (6067866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b0b98df7e01c28c9f664ee59268827a69c3c79c171a02b02ffef9228b6f51`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 1.2 MB (1159980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ee7662f86e2b1be0d4fe7186bad48ae5e8ca0139df09176f358d98cb0cf79`  
		Last Modified: Tue, 04 Oct 2022 21:25:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:df36211ea8e22d85aa48a71f47b84e71075e5cd4cff8a7bd56e32d39ac40b9f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127985085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b13b26f783107c940301d0a957e2aee82d9ad5c03d4c4ae555a58842cadfd88`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:54:14 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:55:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:55:51 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:55:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:55:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:55:53 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:23:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:23:07 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:23:08 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:23:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:23:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:23:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:23:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4c96e872d58125e8e270e7f4c23f0001b8b8b8e32cd703fda75a7bd5ea6a63`  
		Last Modified: Tue, 04 Oct 2022 20:04:46 GMT  
		Size: 116.8 MB (116819377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d612e3ed75f66cf36584943357bb01e4c52945cae40319c28839a9d2993ab8`  
		Last Modified: Tue, 04 Oct 2022 20:04:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8636190f09c5dea38074348308fbd34bc62d9cdce351d95d15bea5504394e3b3`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 7.1 MB (7052392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf5d35a9434ec361ff62efef87605c4eedf5e5ba36f33b45e62d98b79700a5c`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 1.1 MB (1120445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a19533d345cf495d46b1b208b6ea2871a911516c987dc33830e8c6dbad4de2`  
		Last Modified: Tue, 04 Oct 2022 20:23:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:dcf7bef383bc2ef1a9c06670f66c301437106cf6024797255490daa02015f496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128881670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfde85aab958fe6830006ee81bca416ae8dcd25d1b9dde9852c1fdc4b3e01b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:18 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:43:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:43:10 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:43:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:43:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:43:11 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:14:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:14:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:14:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:14:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f162d01985672827ddfb048d004dd524a6cf77a6564ccec1a1b2bb1ca70870`  
		Last Modified: Tue, 04 Oct 2022 19:55:34 GMT  
		Size: 117.2 MB (117204653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c83a388b1d0281151c0ad223e2882ab7835560f24ff8632c6b5572bd52017`  
		Last Modified: Tue, 04 Oct 2022 19:55:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8f0ceb0d32500e04e62486c61d02503e801fb4f11e716eee78234b59f10881`  
		Last Modified: Tue, 04 Oct 2022 20:15:00 GMT  
		Size: 7.5 MB (7482404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a10426e8126ad610a88c0c67c544ec6ad934ba8727e6f432800b5ff279cd11`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 1.1 MB (1103844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11669aeca9837785668f17d866c23756bc9c3978df3d5e84476f32565fd2e589`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:404f3025fa1bf713807ae106c84550d7cc438726dc68e06a917dd9a2999bc0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131828807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528fbc52d70c938ac901a877c243b4ddf059ab8e5071d26ed00c4cb598a58a4b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:51:13 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:53:48 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:53:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:53:49 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:24:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:24:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:24:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:24:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1238bfd151683573cd911e00a0ecb201b2a754f39b8a62e7d0cfe908734d31`  
		Last Modified: Tue, 04 Oct 2022 20:06:50 GMT  
		Size: 120.7 MB (120732088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c161868cfaa1386086f2ebfb88351c233b6b6c0db49a37ae9f06fc971270abce`  
		Last Modified: Tue, 04 Oct 2022 20:06:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20be2863c9fe0842a12f57089063e87713658c0acb8656e230a988f99cdefa`  
		Last Modified: Tue, 04 Oct 2022 20:25:07 GMT  
		Size: 7.1 MB (7053038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5842247ede61565ac01c0eccc30149d27e311f6aa7f3a7ad20c56fbb247ffb2`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 1.2 MB (1167425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a54f79a30bd281d6df17484fdc97e05e169cf138a5b2eff5ebb6932bcd26249`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:21dbf9101c1eae0e2228f386eefab509d462710c2da97ba45d61c083f3e74fc1
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
$ docker pull caddy@sha256:c5422fb96d5bf458fc8a8813354de04ef89cdd6750464608c1a79fa516cb3cf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8159c96a82a85a24bdca751327835b2f572ba3db71f048bfd2a99157c4552a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:21:13 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:21:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:21:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:21:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:21:18 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:21:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4205233f1134d23e80cfe1162f65ddc45f5e08ff0e9b0e8e1f567f1df4868e`  
		Last Modified: Thu, 22 Sep 2022 19:21:41 GMT  
		Size: 14.5 MB (14493827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f35320fa0aa0bd407da7446a532e6bb6ff70ffbbb64aba575f0a6e21ccf51ec`  
		Last Modified: Thu, 22 Sep 2022 19:21:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f2137bdd4a839a19e28becbea0f246fc4597f1d94b9160bbab8d33833a94516a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee668f0f22cd21b96db6834820ac6a8bb48c7e2d0692acea4d45c8da330025c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:49:21 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:49:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:49:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:49:25 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:49:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4bd7a61e1d1d31bb0b5d056e1977f00c6f0b8163f84ac2cc68e852646f3dc3`  
		Last Modified: Thu, 22 Sep 2022 18:50:11 GMT  
		Size: 13.8 MB (13848650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073c127573b2fd3ee6b12c32facd1130f8cc0bea38341433a9964b9284cbf7e`  
		Last Modified: Thu, 22 Sep 2022 18:50:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:754a4ef354849e835ad2f064371f199e12d40bd3a80e2762021dbd80fef7c09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd21ed1eea16f7633d2d018d09b22db42d8bb871a5e2766b2035dc2f9bf68a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:57:20 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:57:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:57:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:57:24 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff391a21d5bd9ec72ea8acc2167c33b229a59f8d895b07f936d10a36f933f85c`  
		Last Modified: Thu, 22 Sep 2022 18:58:08 GMT  
		Size: 13.8 MB (13824532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a0ca8c098350a18188ff1d9a504f8f26fa2877de27bf3da050a0b944f8332`  
		Last Modified: Thu, 22 Sep 2022 18:58:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:91ec6f75105a515495f3e158f4ca7330acf40f7853f554551c083988c668d3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fd3ed314bb850c421d68a78109b3a91fefc6042029dbf260b55437858a1226`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:41:41 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:41:48 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:41:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:41:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:41:56 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:41:57 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:41:58 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:41:59 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:42:00 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:42:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173eaf2f5d3a64c1a049b7d37dae2bd5b53c6523dae94e9d5aa27953c5b6f2a`  
		Last Modified: Thu, 22 Sep 2022 19:42:44 GMT  
		Size: 13.2 MB (13196254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa836aafb15eb36353931beffa1076de802cab80de1ac30f53fe21aca65c6768`  
		Last Modified: Thu, 22 Sep 2022 19:42:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b7f03acd5c95c3455c9ce665785094ab0a08a757428c633d02b38e88204d533b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89193f536932af1c50b869234fb5354966b6af6bae71497c49c9bd2ba58e8d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:16:17 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:16:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:26 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:16:26 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:16:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57cf77fded040254299e259088c60baca34a7b637739623d4ef8b6e1aee8cc`  
		Last Modified: Thu, 22 Sep 2022 19:17:11 GMT  
		Size: 12.9 MB (12853691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060df16a418309fc2e3f0b60e8eec07b0aff8301ea214986b2e52de5ed766b28`  
		Last Modified: Thu, 22 Sep 2022 19:17:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:f0302c1158b1f1012c28e30a9f5f34321025ddf9c1f604f3a329b2014594e3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc35bb304c92287f0aa42f10af772c3fcb2086ccddb60f4329be61f6abc43c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:03:35 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:03:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:03:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:03:42 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:03:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cecf0b1f1e9b6a8368ba9be6a20e436697da448defc79dc55108e9ea5629d5`  
		Last Modified: Thu, 22 Sep 2022 19:04:54 GMT  
		Size: 14.0 MB (14001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139004284fd2d833d52451b088c4156944f30e57982c6f6d2a73afddbd1d8679`  
		Last Modified: Thu, 22 Sep 2022 19:04:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:7074b59735ddf6643ff6d00f59901a9c46478911fb6f0b8a83218e8a755cd7dc
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
$ docker pull caddy@sha256:806531835a3ee4b98692120ba7d5d77ac9f67511336e958a94e3549835582506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133499962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd36cbedf423aed317a7e06e0972147588fccb7de574399071068df83b945ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:54 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:42:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:42:33 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:42:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:42:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:42:34 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:09:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:09:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:09:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:09:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d81b0672f0319abbe5d231bb316a758f235e12071775381065b3b787f6121`  
		Last Modified: Tue, 04 Oct 2022 19:51:00 GMT  
		Size: 122.3 MB (122251625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277b443bd1a959724dd2b3a89b8e8543f8a7de36f62be65f2126b879ad5c8ad`  
		Last Modified: Tue, 04 Oct 2022 19:50:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c8786f0992e8dd727c0222b7d05611f30c7eca1bbaeda8313d28a5e718b541`  
		Last Modified: Tue, 04 Oct 2022 20:09:36 GMT  
		Size: 6.9 MB (6941670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8144098c5e0f2da20fdee70369ed4ae79b2b710c60dac6da94801fa9c8c1cc`  
		Last Modified: Tue, 04 Oct 2022 20:09:35 GMT  
		Size: 1.2 MB (1215172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfff0203e2ac04ac7edadd406708b3360bfc6bd4ebb109b85827a4eb9f177f8`  
		Last Modified: Tue, 04 Oct 2022 20:09:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f73afa45a85262dc63d4d983ab2da8e0eead8b7760f0039c199e732fca5885ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638a32ec67f67b37f9cb0d65ae80161b7823754208317f3342c25b1d40b5ee3c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:39:35 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:49:16 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:49:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:49:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:49:17 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:30:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:30:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:30:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d349e0f4f9311c744c13786b11824154e1c08216ad948d5ebe82875cb878bd7`  
		Last Modified: Tue, 04 Oct 2022 20:12:32 GMT  
		Size: 118.6 MB (118635919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf625d0f07ffea6400b4db19ae8153464917f23dbf61749929881eeb2b37fb8`  
		Last Modified: Tue, 04 Oct 2022 20:12:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e7fcc5c56e0e9828396fa37456be04a382caec3623869e4e66da9790681e6`  
		Last Modified: Tue, 04 Oct 2022 20:31:23 GMT  
		Size: 6.8 MB (6808221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c653d47fa466da3e7b3a3bd7f075c55ff07045cd227a53eae150d5bdd295c1b`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 1.2 MB (1162979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96ffbe114ba0a9a2f25781826343ada15f29699fd17e821c3afd6dc66b3072`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9c9aa1fce6c5b5cfcd3653fff55bdbbcf2ef34bac0a2e82dc6fe2d7a452fb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0067bb4da6d1523159ac91a84a2efae963acb89737ee757ad59cbcd16937a71f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:51 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 20:02:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 20:02:23 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 20:02:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 20:02:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 20:02:24 GMT
WORKDIR /go
# Tue, 04 Oct 2022 21:25:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 21:25:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 21:25:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 21:25:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371376b3d092072c91d12b8ae8b6d7c23dd222982378385554faee7555afbc9`  
		Last Modified: Tue, 04 Oct 2022 20:21:44 GMT  
		Size: 118.4 MB (118407284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed516331f5140684e05fdce25e0c0295e18775b343abe2bc63e1bb63c421d868`  
		Last Modified: Tue, 04 Oct 2022 20:21:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa31122002e131a4f100cc84e1f6b72b13c4b1f04381ac5498c42f9781284b`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 6.1 MB (6067866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b0b98df7e01c28c9f664ee59268827a69c3c79c171a02b02ffef9228b6f51`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 1.2 MB (1159980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ee7662f86e2b1be0d4fe7186bad48ae5e8ca0139df09176f358d98cb0cf79`  
		Last Modified: Tue, 04 Oct 2022 21:25:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:df36211ea8e22d85aa48a71f47b84e71075e5cd4cff8a7bd56e32d39ac40b9f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127985085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b13b26f783107c940301d0a957e2aee82d9ad5c03d4c4ae555a58842cadfd88`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:54:14 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:55:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:55:51 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:55:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:55:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:55:53 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:23:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:23:07 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:23:08 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:23:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:23:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:23:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:23:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4c96e872d58125e8e270e7f4c23f0001b8b8b8e32cd703fda75a7bd5ea6a63`  
		Last Modified: Tue, 04 Oct 2022 20:04:46 GMT  
		Size: 116.8 MB (116819377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d612e3ed75f66cf36584943357bb01e4c52945cae40319c28839a9d2993ab8`  
		Last Modified: Tue, 04 Oct 2022 20:04:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8636190f09c5dea38074348308fbd34bc62d9cdce351d95d15bea5504394e3b3`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 7.1 MB (7052392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf5d35a9434ec361ff62efef87605c4eedf5e5ba36f33b45e62d98b79700a5c`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 1.1 MB (1120445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a19533d345cf495d46b1b208b6ea2871a911516c987dc33830e8c6dbad4de2`  
		Last Modified: Tue, 04 Oct 2022 20:23:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:dcf7bef383bc2ef1a9c06670f66c301437106cf6024797255490daa02015f496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128881670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfde85aab958fe6830006ee81bca416ae8dcd25d1b9dde9852c1fdc4b3e01b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:18 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:43:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:43:10 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:43:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:43:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:43:11 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:14:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:14:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:14:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:14:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f162d01985672827ddfb048d004dd524a6cf77a6564ccec1a1b2bb1ca70870`  
		Last Modified: Tue, 04 Oct 2022 19:55:34 GMT  
		Size: 117.2 MB (117204653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c83a388b1d0281151c0ad223e2882ab7835560f24ff8632c6b5572bd52017`  
		Last Modified: Tue, 04 Oct 2022 19:55:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8f0ceb0d32500e04e62486c61d02503e801fb4f11e716eee78234b59f10881`  
		Last Modified: Tue, 04 Oct 2022 20:15:00 GMT  
		Size: 7.5 MB (7482404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a10426e8126ad610a88c0c67c544ec6ad934ba8727e6f432800b5ff279cd11`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 1.1 MB (1103844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11669aeca9837785668f17d866c23756bc9c3978df3d5e84476f32565fd2e589`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:404f3025fa1bf713807ae106c84550d7cc438726dc68e06a917dd9a2999bc0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131828807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528fbc52d70c938ac901a877c243b4ddf059ab8e5071d26ed00c4cb598a58a4b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:51:13 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:53:48 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:53:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:53:49 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:24:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:24:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:24:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:24:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1238bfd151683573cd911e00a0ecb201b2a754f39b8a62e7d0cfe908734d31`  
		Last Modified: Tue, 04 Oct 2022 20:06:50 GMT  
		Size: 120.7 MB (120732088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c161868cfaa1386086f2ebfb88351c233b6b6c0db49a37ae9f06fc971270abce`  
		Last Modified: Tue, 04 Oct 2022 20:06:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20be2863c9fe0842a12f57089063e87713658c0acb8656e230a988f99cdefa`  
		Last Modified: Tue, 04 Oct 2022 20:25:07 GMT  
		Size: 7.1 MB (7053038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5842247ede61565ac01c0eccc30149d27e311f6aa7f3a7ad20c56fbb247ffb2`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 1.2 MB (1167425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a54f79a30bd281d6df17484fdc97e05e169cf138a5b2eff5ebb6932bcd26249`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:8106c25f6910ae0302bffc6b16ae6e8a7d9a9a4cd90d3e8007a7856b5c2d82eb
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
$ docker pull caddy@sha256:806531835a3ee4b98692120ba7d5d77ac9f67511336e958a94e3549835582506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133499962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd36cbedf423aed317a7e06e0972147588fccb7de574399071068df83b945ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:54 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:42:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:42:33 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:42:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:42:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:42:34 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:09:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:09:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:09:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:09:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:09:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d81b0672f0319abbe5d231bb316a758f235e12071775381065b3b787f6121`  
		Last Modified: Tue, 04 Oct 2022 19:51:00 GMT  
		Size: 122.3 MB (122251625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277b443bd1a959724dd2b3a89b8e8543f8a7de36f62be65f2126b879ad5c8ad`  
		Last Modified: Tue, 04 Oct 2022 19:50:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c8786f0992e8dd727c0222b7d05611f30c7eca1bbaeda8313d28a5e718b541`  
		Last Modified: Tue, 04 Oct 2022 20:09:36 GMT  
		Size: 6.9 MB (6941670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8144098c5e0f2da20fdee70369ed4ae79b2b710c60dac6da94801fa9c8c1cc`  
		Last Modified: Tue, 04 Oct 2022 20:09:35 GMT  
		Size: 1.2 MB (1215172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfff0203e2ac04ac7edadd406708b3360bfc6bd4ebb109b85827a4eb9f177f8`  
		Last Modified: Tue, 04 Oct 2022 20:09:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f73afa45a85262dc63d4d983ab2da8e0eead8b7760f0039c199e732fca5885ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638a32ec67f67b37f9cb0d65ae80161b7823754208317f3342c25b1d40b5ee3c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:39:35 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:49:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:49:16 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:49:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:49:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:49:17 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:30:41 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:30:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:30:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:30:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d349e0f4f9311c744c13786b11824154e1c08216ad948d5ebe82875cb878bd7`  
		Last Modified: Tue, 04 Oct 2022 20:12:32 GMT  
		Size: 118.6 MB (118635919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf625d0f07ffea6400b4db19ae8153464917f23dbf61749929881eeb2b37fb8`  
		Last Modified: Tue, 04 Oct 2022 20:12:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e7fcc5c56e0e9828396fa37456be04a382caec3623869e4e66da9790681e6`  
		Last Modified: Tue, 04 Oct 2022 20:31:23 GMT  
		Size: 6.8 MB (6808221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c653d47fa466da3e7b3a3bd7f075c55ff07045cd227a53eae150d5bdd295c1b`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 1.2 MB (1162979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96ffbe114ba0a9a2f25781826343ada15f29699fd17e821c3afd6dc66b3072`  
		Last Modified: Tue, 04 Oct 2022 20:31:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9c9aa1fce6c5b5cfcd3653fff55bdbbcf2ef34bac0a2e82dc6fe2d7a452fb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128336726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0067bb4da6d1523159ac91a84a2efae963acb89737ee757ad59cbcd16937a71f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:51 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 20:02:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 20:02:23 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 20:02:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 20:02:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 20:02:24 GMT
WORKDIR /go
# Tue, 04 Oct 2022 21:25:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 21:25:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 21:25:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 21:25:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 21:25:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371376b3d092072c91d12b8ae8b6d7c23dd222982378385554faee7555afbc9`  
		Last Modified: Tue, 04 Oct 2022 20:21:44 GMT  
		Size: 118.4 MB (118407284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed516331f5140684e05fdce25e0c0295e18775b343abe2bc63e1bb63c421d868`  
		Last Modified: Tue, 04 Oct 2022 20:21:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa31122002e131a4f100cc84e1f6b72b13c4b1f04381ac5498c42f9781284b`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 6.1 MB (6067866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b0b98df7e01c28c9f664ee59268827a69c3c79c171a02b02ffef9228b6f51`  
		Last Modified: Tue, 04 Oct 2022 21:25:41 GMT  
		Size: 1.2 MB (1159980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ee7662f86e2b1be0d4fe7186bad48ae5e8ca0139df09176f358d98cb0cf79`  
		Last Modified: Tue, 04 Oct 2022 21:25:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:df36211ea8e22d85aa48a71f47b84e71075e5cd4cff8a7bd56e32d39ac40b9f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127985085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b13b26f783107c940301d0a957e2aee82d9ad5c03d4c4ae555a58842cadfd88`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:54:14 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:55:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:55:51 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:55:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:55:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:55:53 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:23:06 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:23:07 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:23:08 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:23:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:23:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:23:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:23:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4c96e872d58125e8e270e7f4c23f0001b8b8b8e32cd703fda75a7bd5ea6a63`  
		Last Modified: Tue, 04 Oct 2022 20:04:46 GMT  
		Size: 116.8 MB (116819377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d612e3ed75f66cf36584943357bb01e4c52945cae40319c28839a9d2993ab8`  
		Last Modified: Tue, 04 Oct 2022 20:04:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8636190f09c5dea38074348308fbd34bc62d9cdce351d95d15bea5504394e3b3`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 7.1 MB (7052392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf5d35a9434ec361ff62efef87605c4eedf5e5ba36f33b45e62d98b79700a5c`  
		Last Modified: Tue, 04 Oct 2022 20:23:45 GMT  
		Size: 1.1 MB (1120445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a19533d345cf495d46b1b208b6ea2871a911516c987dc33830e8c6dbad4de2`  
		Last Modified: Tue, 04 Oct 2022 20:23:44 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:dcf7bef383bc2ef1a9c06670f66c301437106cf6024797255490daa02015f496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128881670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfde85aab958fe6830006ee81bca416ae8dcd25d1b9dde9852c1fdc4b3e01b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:40:18 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:43:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:43:10 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:43:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:43:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:43:11 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:14:17 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:14:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:14:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:14:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:14:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f162d01985672827ddfb048d004dd524a6cf77a6564ccec1a1b2bb1ca70870`  
		Last Modified: Tue, 04 Oct 2022 19:55:34 GMT  
		Size: 117.2 MB (117204653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c83a388b1d0281151c0ad223e2882ab7835560f24ff8632c6b5572bd52017`  
		Last Modified: Tue, 04 Oct 2022 19:55:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8f0ceb0d32500e04e62486c61d02503e801fb4f11e716eee78234b59f10881`  
		Last Modified: Tue, 04 Oct 2022 20:15:00 GMT  
		Size: 7.5 MB (7482404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a10426e8126ad610a88c0c67c544ec6ad934ba8727e6f432800b5ff279cd11`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 1.1 MB (1103844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11669aeca9837785668f17d866c23756bc9c3978df3d5e84476f32565fd2e589`  
		Last Modified: Tue, 04 Oct 2022 20:14:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:404f3025fa1bf713807ae106c84550d7cc438726dc68e06a917dd9a2999bc0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131828807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528fbc52d70c938ac901a877c243b4ddf059ab8e5071d26ed00c4cb598a58a4b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:51:13 GMT
ENV GOLANG_VERSION=1.19.2
# Tue, 04 Oct 2022 19:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.2.src.tar.gz'; 		sha256='2ce930d70a931de660fdaf271d70192793b1b240272645bf0275779f6704df6b'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Oct 2022 19:53:48 GMT
ENV GOPATH=/go
# Tue, 04 Oct 2022 19:53:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 19:53:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 04 Oct 2022 19:53:49 GMT
WORKDIR /go
# Tue, 04 Oct 2022 20:24:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV CADDY_VERSION=v2.6.1
# Tue, 04 Oct 2022 20:24:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Oct 2022 20:24:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Oct 2022 20:24:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Oct 2022 20:24:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1238bfd151683573cd911e00a0ecb201b2a754f39b8a62e7d0cfe908734d31`  
		Last Modified: Tue, 04 Oct 2022 20:06:50 GMT  
		Size: 120.7 MB (120732088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c161868cfaa1386086f2ebfb88351c233b6b6c0db49a37ae9f06fc971270abce`  
		Last Modified: Tue, 04 Oct 2022 20:06:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c20be2863c9fe0842a12f57089063e87713658c0acb8656e230a988f99cdefa`  
		Last Modified: Tue, 04 Oct 2022 20:25:07 GMT  
		Size: 7.1 MB (7053038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5842247ede61565ac01c0eccc30149d27e311f6aa7f3a7ad20c56fbb247ffb2`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 1.2 MB (1167425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a54f79a30bd281d6df17484fdc97e05e169cf138a5b2eff5ebb6932bcd26249`  
		Last Modified: Tue, 04 Oct 2022 20:25:06 GMT  
		Size: 405.0 B  
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
$ docker pull caddy@sha256:faadebac07e5c9daaa97adf528801d228c01d706a6755ab0c082acc4702e25de
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
$ docker pull caddy@sha256:c5422fb96d5bf458fc8a8813354de04ef89cdd6750464608c1a79fa516cb3cf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17610375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8159c96a82a85a24bdca751327835b2f572ba3db71f048bfd2a99157c4552a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:21:13 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:21:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:21:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:21:17 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:21:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:21:17 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:21:18 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:21:18 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:21:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56da4be4f98aabf384c325fdd5372f380cd5105a18d7cdea0932b91c5dd929e`  
		Last Modified: Wed, 07 Sep 2022 21:20:20 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4205233f1134d23e80cfe1162f65ddc45f5e08ff0e9b0e8e1f567f1df4868e`  
		Last Modified: Thu, 22 Sep 2022 19:21:41 GMT  
		Size: 14.5 MB (14493827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f35320fa0aa0bd407da7446a532e6bb6ff70ffbbb64aba575f0a6e21ccf51ec`  
		Last Modified: Thu, 22 Sep 2022 19:21:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f2137bdd4a839a19e28becbea0f246fc4597f1d94b9160bbab8d33833a94516a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16773071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee668f0f22cd21b96db6834820ac6a8bb48c7e2d0692acea4d45c8da330025c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:49:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:49:21 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:49:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:49:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:49:24 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:49:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:49:25 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:49:25 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:49:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db7c4c704a51c96221735c509db9b19c8d834850bca0524cbaae017616448d`  
		Last Modified: Wed, 07 Sep 2022 20:50:58 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4bd7a61e1d1d31bb0b5d056e1977f00c6f0b8163f84ac2cc68e852646f3dc3`  
		Last Modified: Thu, 22 Sep 2022 18:50:11 GMT  
		Size: 13.8 MB (13848650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073c127573b2fd3ee6b12c32facd1130f8cc0bea38341433a9964b9284cbf7e`  
		Last Modified: Thu, 22 Sep 2022 18:50:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:754a4ef354849e835ad2f064371f199e12d40bd3a80e2762021dbd80fef7c09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16551191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd21ed1eea16f7633d2d018d09b22db42d8bb871a5e2766b2035dc2f9bf68a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:57:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 18:57:20 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 18:57:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 18:57:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 18:57:23 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 18:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 18:57:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 80
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 18:57:24 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 18:57:24 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 18:57:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86dff9c253b1ffb3d594359a267c83d2bf72743dcedb6c66204eb333fb3ab17`  
		Last Modified: Wed, 07 Sep 2022 20:59:22 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff391a21d5bd9ec72ea8acc2167c33b229a59f8d895b07f936d10a36f933f85c`  
		Last Modified: Thu, 22 Sep 2022 18:58:08 GMT  
		Size: 13.8 MB (13824532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6a0ca8c098350a18188ff1d9a504f8f26fa2877de27bf3da050a0b944f8332`  
		Last Modified: Thu, 22 Sep 2022 18:58:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:91ec6f75105a515495f3e158f4ca7330acf40f7853f554551c083988c668d3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16214123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fd3ed314bb850c421d68a78109b3a91fefc6042029dbf260b55437858a1226`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:39:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:41:41 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:41:48 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:41:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:41:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:41:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:41:56 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:41:57 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:41:58 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:41:59 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:42:00 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:42:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba9cfa79ccdc607f6ea641b7c94062532f81975ebd5419bf068d1fe2af960e`  
		Last Modified: Wed, 07 Sep 2022 20:41:25 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6173eaf2f5d3a64c1a049b7d37dae2bd5b53c6523dae94e9d5aa27953c5b6f2a`  
		Last Modified: Thu, 22 Sep 2022 19:42:44 GMT  
		Size: 13.2 MB (13196254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa836aafb15eb36353931beffa1076de802cab80de1ac30f53fe21aca65c6768`  
		Last Modified: Thu, 22 Sep 2022 19:42:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:b7f03acd5c95c3455c9ce665785094ab0a08a757428c633d02b38e88204d533b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15969503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89193f536932af1c50b869234fb5354966b6af6bae71497c49c9bd2ba58e8d4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 21:16:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:16:17 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:16:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:16:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:16:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:16:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:16:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:16:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:16:25 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:16:26 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:16:26 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:16:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da169c2577ab0c1ae68129fab3202e2c87c9010f5651350ba9eae373d6a379`  
		Last Modified: Wed, 07 Sep 2022 21:18:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff57cf77fded040254299e259088c60baca34a7b637739623d4ef8b6e1aee8cc`  
		Last Modified: Thu, 22 Sep 2022 19:17:11 GMT  
		Size: 12.9 MB (12853691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060df16a418309fc2e3f0b60e8eec07b0aff8301ea214986b2e52de5ed766b28`  
		Last Modified: Thu, 22 Sep 2022 19:17:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:f0302c1158b1f1012c28e30a9f5f34321025ddf9c1f604f3a329b2014594e3a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16902901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc35bb304c92287f0aa42f10af772c3fcb2086ccddb60f4329be61f6abc43c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 07 Sep 2022 20:41:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 22 Sep 2022 19:03:35 GMT
ENV CADDY_VERSION=v2.6.1
# Thu, 22 Sep 2022 19:03:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='fc0c0c115ad0f4e7ca5622dedb95c5c4bc5fc5a44731aa63c6cbc6307d3e6dfe3ae040d6580e2064c5c84bded165c768cac0125fdb9418c923272ccd7fdf19ed' ;; 		armhf)   binArch='armv6'; checksum='9aa52d748e45069ce15274b09737e5806b5aa355c4e32cdc187d478bdd5c1cf22398e0ac365933f64386d79b11860246b8340a740a25644a8bfa6ed032bc5b2f' ;; 		armv7)   binArch='armv7'; checksum='d5b026c9f6d4f2aeb9058d6d990d6420439985bd8cbb18f028c6adc7f6a22d3d28a6478958117dbb5051d6537f3b8a9bb61ec8cfa631e33032c7000fa0c44c83' ;; 		aarch64) binArch='arm64'; checksum='92a2310ba12a790d632a288c285c2aa7be16eb3521212f78644c07d1c65d7f27ec81823a10e7ea4a200a013cb557d335a06c95c94fdf1f2359f47f4974b6e37a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c12b3660a7cf0b359d8153bc6be4b7dedf1168e7984fccbf6cf804abaefcbf5edd10651de6c0f7541e8eaefbcdc25eb00b5c2500b8b445e7f8a9382e0fa3ced1' ;; 		s390x)   binArch='s390x'; checksum='da1d8d60547de3122603134394b3e2bbe18b7fbecc0bba0d24352c7dd765bec6f2cadc93b00ae69369f14e1800a2318cc94af3ab940710a622bf7be4f713bf0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.1/caddy_2.6.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 22 Sep 2022 19:03:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 22 Sep 2022 19:03:40 GMT
ENV XDG_DATA_HOME=/data
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.version=v2.6.1
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 22 Sep 2022 19:03:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 22 Sep 2022 19:03:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 80
# Thu, 22 Sep 2022 19:03:41 GMT
EXPOSE 443
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 443/udp
# Thu, 22 Sep 2022 19:03:42 GMT
EXPOSE 2019
# Thu, 22 Sep 2022 19:03:42 GMT
WORKDIR /srv
# Thu, 22 Sep 2022 19:03:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244aa99ed48fdbb566d90b862044c3d5a2b205d096efe5fd1e58257b140ea7cc`  
		Last Modified: Wed, 07 Sep 2022 20:42:58 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cecf0b1f1e9b6a8368ba9be6a20e436697da448defc79dc55108e9ea5629d5`  
		Last Modified: Thu, 22 Sep 2022 19:04:54 GMT  
		Size: 14.0 MB (14001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139004284fd2d833d52451b088c4156944f30e57982c6f6d2a73afddbd1d8679`  
		Last Modified: Thu, 22 Sep 2022 19:04:48 GMT  
		Size: 155.0 B  
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
