<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.1.1`](#caddy211)
-	[`caddy:2.1.1-alpine`](#caddy211-alpine)
-	[`caddy:2.1.1-builder`](#caddy211-builder)
-	[`caddy:2.1.1-builder-alpine`](#caddy211-builder-alpine)
-	[`caddy:2.1.1-builder-windowsservercore-1809`](#caddy211-builder-windowsservercore-1809)
-	[`caddy:2.1.1-builder-windowsservercore-ltsc2016`](#caddy211-builder-windowsservercore-ltsc2016)
-	[`caddy:2.1.1-windowsservercore`](#caddy211-windowsservercore)
-	[`caddy:2.1.1-windowsservercore-1809`](#caddy211-windowsservercore-1809)
-	[`caddy:2.1.1-windowsservercore-ltsc2016`](#caddy211-windowsservercore-ltsc2016)
-	[`caddy:2.2.0`](#caddy220)
-	[`caddy:2.2.0-alpine`](#caddy220-alpine)
-	[`caddy:2.2.0-builder`](#caddy220-builder)
-	[`caddy:2.2.0-builder-alpine`](#caddy220-builder-alpine)
-	[`caddy:2.2.0-builder-windowsservercore-1809`](#caddy220-builder-windowsservercore-1809)
-	[`caddy:2.2.0-builder-windowsservercore-ltsc2016`](#caddy220-builder-windowsservercore-ltsc2016)
-	[`caddy:2.2.0-windowsservercore`](#caddy220-windowsservercore)
-	[`caddy:2.2.0-windowsservercore-1809`](#caddy220-windowsservercore-1809)
-	[`caddy:2.2.0-windowsservercore-ltsc2016`](#caddy220-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:878e0f076a0c34ddf9f15af052a4fd802aa5b7e69393582655a4fa3755876db8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:7210e033f1b7846a51ad4e7e0412f5eecff286aa706500698fbea1f89c316357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14632306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6f01784bcc9de68ae349a8c782c82c8d54f642f6cbadb2472567ea33e69cf0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:27:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:35 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:36 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:38 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bea3a62f2eb8bdd91cf1d01de5e62aa88dbcd8e5834f5dd686a4f1a482531`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 5.8 KB (5761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c6d72ce944f51161d2c13a01dde2210e77bb69c72cbd54e3125a34d60d899`  
		Last Modified: Fri, 25 Sep 2020 22:28:11 GMT  
		Size: 11.5 MB (11528869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e626bfeb2f84ef9a852704892ac16a98c0562469db9c76430725e5c18a998ddb`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c8ad488eec7c77aa1c7781b7a72a8d945481bdd0cb7ccb70880d9b925873048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f98716bd7a8a9c2ef8aa29c6650238e67c38bdb8293c65fee78840359abf69`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:50:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:50:11 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:50:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:50:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:50:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:50:20 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:50:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:50:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:50:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:50:27 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:50:28 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:50:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf9fef63ad932b076740c7fd4eac18d505c2e815b2b27093fae4a1037c1f83`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4febe5cd2333cc513bb8556e642ebf16c47e8b19d55ca0a5ea133b0ac51ffb6`  
		Last Modified: Fri, 25 Sep 2020 22:51:22 GMT  
		Size: 10.9 MB (10871161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a4a456aa5012b57a14ca79cf84c1fcadb9921dacbceabaa51276b470026164`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f7cf9f964eeea33eafd618e61be6df5924aeb7554b18ebf67553d7b6b4b87c4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13563595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9c246982f6b6958d5da2a3fd34536f8ac51c0bb7d8b9f5dac90402a50362ae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:58:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:58:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:58:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:58:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:58:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:58:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:58:40 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:58:41 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:42 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:51 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f21378d6028fa7cda0d5b592cd8b633c405139cc47eee9863c2b21da4378b`  
		Last Modified: Fri, 25 Sep 2020 22:59:48 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665bdf05fdd3470eab6a6ffbc672a036b9fd454b448b462f016d7ca8ef6948`  
		Last Modified: Fri, 25 Sep 2020 22:59:51 GMT  
		Size: 10.9 MB (10851606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff23fb2f1e176ebd5c38157ac164416de40bede15eda73c657fcd72ab44cbf4`  
		Last Modified: Fri, 25 Sep 2020 22:59:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fd7be1e3e7e8f22025c4c7c932ed959e20a042800583b99d221d49210d2256b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13537918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdda1ab60a0a087288e1096da6b835d6d0492ace07c13f12b7ae57fc0aa31fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:18 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:40:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:40:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:40:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:40:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:40:26 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:40:27 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:40:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:40:33 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:40:34 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:40:35 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:40:35 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:40:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bbc79642b3dde186ddb45804729b84a8d010ca521d5c376311e2f613371675`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737d74b46f3ab6089d70958b2003334d319108e095e574ccb5513b8df65957b`  
		Last Modified: Fri, 25 Sep 2020 22:41:26 GMT  
		Size: 10.5 MB (10523576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bccfced4019a7c0a8f4727d9564f261cc2cea2f152604c090c8e1534648917`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:1f9ba55d19fd2ec980dbaeab620562f227dcf0d7ced312dc989d275783c346eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13288765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3fce9822eca46a2dd633cf719e3ed86a1381b29ecaf6869f8959e53899d0e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:41 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:09 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:38 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:47 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:42:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:42:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:42:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:42:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:42:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:42:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:42:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:42:53 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:42:59 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:43:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6899a5c1a337a29052e5f09180d092a86821dcf3d513b96fdf5db876ec3d6368`  
		Last Modified: Fri, 25 Sep 2020 22:45:34 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5fe5c56024bfb32687701ff11f9c64f76889469f8562abad35c6b11862a8cb`  
		Last Modified: Fri, 25 Sep 2020 22:45:35 GMT  
		Size: 10.2 MB (10175209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09e4037c29b877b9d6dc22577ae3f8283f506d76525794858646d23a4c596`  
		Last Modified: Fri, 25 Sep 2020 22:45:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:aab2bff384d7eeaac65e97fe65c9f60f11a3515ae789192681455c483e7849d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14069343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036d0863bbc70fc945f1013ac5fc1b1ffa1f292eafc9e5cb9b6167ae03031199`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:41:44 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:50 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b62d245db5345045e7a29f409c7a0109545e93366793659a9538d863745398`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd84433ce0180dc40fb2dfc528d8186c247a35a24b5868a7b6065989bf0ee684`  
		Last Modified: Fri, 25 Sep 2020 22:42:26 GMT  
		Size: 11.2 MB (11196639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b4a42908e611c3b87202fd7fa709303806890837e261ae5a76d427925c7825`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

```console
$ docker pull caddy@sha256:36d33821209e5584d44597f773fde5bd4bd002296ac7a663140df706f6fde183
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.1.1` - linux; amd64

```console
$ docker pull caddy@sha256:80d608bfebf1d919d7613d401af6004ba74a3be96867e1a25d9ab35a2da6714f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fd8ade3df48988e09df79afd3361daa868169892daa8efc4b9b88028fada48a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:27:13 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:27:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:16 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:16 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:17 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:18 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:18 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:19 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:19 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff8cd7408716264fcaa599bf31e94490e2cf2281ce3d87c7376ecaabf995f2c`  
		Last Modified: Fri, 25 Sep 2020 22:27:59 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445f33e99ec338357aded23d1cf928a75a2ce5f6c840c49fc4a9469c0de07700`  
		Last Modified: Fri, 25 Sep 2020 22:28:01 GMT  
		Size: 13.1 MB (13057337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2107641907cbbc1ab9d5f92fc706779dfb06fa4f287e29f0e0731d27efab1d`  
		Last Modified: Fri, 25 Sep 2020 22:27:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6a6e8e419c6b07de12627d56e57d7526bbf0b7e0ed6444059310741aa823bf85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32588090d7bb2509380b4739113c43093f60dba0016465ed03143ef0225790e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:49:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:49:30 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:49:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:49:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:49:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:49:38 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:49:39 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:49:39 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:49:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:49:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:49:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:49:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:49:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:49:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:49:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:49:45 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:49:46 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:49:46 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:49:47 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f230a7df78269514af68ed5207d0d2ade5646619012a49f07564abd097a4f43`  
		Last Modified: Fri, 25 Sep 2020 22:51:00 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9826d83e7a201860c01ef0c6b537b3c7b672a109e04dc5e37b58051a7173ec21`  
		Last Modified: Fri, 25 Sep 2020 22:51:05 GMT  
		Size: 12.4 MB (12414930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20425603e5d968a6603537e218e4cc64a53b97498cbaf265bd952b931f6bbea`  
		Last Modified: Fri, 25 Sep 2020 22:51:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1d5c01fc7bfacc51f7d10dcdcb0b6b8de3aac2df9bfd8db586d207d88f2a833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a694089ff1fc1cffa1e5ea27b0ae3f3cf3c40ee1d21bcf6e9eb7ea94352b4fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:57:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:57:50 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:57:58 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:57:59 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:57:59 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:58:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:07 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:08 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c815fe644041cd1e2a8be930b155833108c9af6b9214feb5b1c2f3b1710842af`  
		Last Modified: Fri, 25 Sep 2020 22:59:26 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c03433041ed8c869ebfd10d91d6673d1892324cbad0cdf2bdfb7eedc084a9d`  
		Last Modified: Fri, 25 Sep 2020 22:59:30 GMT  
		Size: 12.4 MB (12396043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8766336719d6750ac25a3c3bb665a18388a58138b4cdf8792ffc8aeb49c0099f`  
		Last Modified: Fri, 25 Sep 2020 22:59:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:04c78db76cedc0f3b4c2133fdc640dd69b1d9899b74b006c122f18352ab5fb1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe2123125accfb26638d3d060043f8032c66ff423f24993e350219facbf429c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:39:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:39:36 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:39:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:39:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:39:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:39:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:39:43 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:39:44 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:39:45 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:39:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:39:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:39:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:39:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:39:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:39:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:39:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:39:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:39:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:39:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:39:52 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:39:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7ce2e195b05936e35a055c73bad445ca921206fd8c0c018f8a9b882488ec1a`  
		Last Modified: Fri, 25 Sep 2020 22:41:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0170c97deb56c282ca48bf564346008e7f0e44767d6e54a3cc25403771f36957`  
		Last Modified: Fri, 25 Sep 2020 22:41:10 GMT  
		Size: 12.0 MB (12013100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f581aff5bd1747039f52bd705bbe5482b368537c82ea8d9ec22c966a97dbc`  
		Last Modified: Fri, 25 Sep 2020 22:41:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:d5fc341e5909164e6d09c5aa91ffea06ecdec40e4ece378e4d20a05ca1ac2d38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67135043576dd821b2eebd66491f6bdf03d306dd63f80ae70348a3a44d12f63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:34:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:34:28 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:34:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:35:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:35:08 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:35:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:35:37 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:35:49 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:36:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:36:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:36:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:36:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:36:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:36:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:37:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:37:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:37:29 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:37:41 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:37:56 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:38:09 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:38:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c2cc7761fc2675da80a24060fc865587f2c860a62a474056465c2402d691f8`  
		Last Modified: Fri, 25 Sep 2020 22:45:07 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98625f8d1b9c837094e190b29036054a427daabf5d3945434b54c89da129cc43`  
		Last Modified: Fri, 25 Sep 2020 22:45:10 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca513b6513d2e7c22c90baf1a8509f6d91cfc20edb99506d72239f7e755d62d`  
		Last Modified: Fri, 25 Sep 2020 22:45:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; s390x

```console
$ docker pull caddy@sha256:20408b3f483d7f32960f3839286b404f633ae99da1e8932dc429bc0c6b3a94b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84cdf8e8f810203a97d0597b2d9f5bab7d5b0eecb14ed3a12237bdea870bf2c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:41:22 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:41:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:26 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:27 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:27 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:41:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:29 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:29 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:29 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:29 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13489b412dcfe7f996349c0742c4bbefde864c19defb8240fa21a95881ea436`  
		Last Modified: Fri, 25 Sep 2020 22:42:11 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe4b720629eafad7b4379d0af34dcfd8d8de2540c694d2e1f420f89b2ee5d68`  
		Last Modified: Fri, 25 Sep 2020 22:42:13 GMT  
		Size: 12.8 MB (12836819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873125611edecc47abc85437ff79cdbf0c56c9d7509ac7e7a3941f87323e9fa4`  
		Last Modified: Fri, 25 Sep 2020 22:42:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:0c81e39f253977e239df5f59cf89da2f5c7f009ce1dab3af9c935b96ace5f111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378453354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b788438493f88710ba4198f5a8e2324ba21a891ac37ad2d9279608278dae239e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:21:26 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:21:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:21:59 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:22:00 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:22:01 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 22:22:01 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 22:22:02 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:22:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:22:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:22:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:22:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:22:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:22:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:22:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:22:07 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:22:08 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:22:09 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:22:23 GMT
RUN caddy version
# Fri, 25 Sep 2020 22:22:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a93d915a3d15febf5cb14d3ce13f84e4e1b59e54251670dffff8c859031c10a`  
		Last Modified: Sat, 26 Sep 2020 00:07:38 GMT  
		Size: 9.2 MB (9161113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af424f647689600c8a89cb1e4745cfc5f8a9ec3fa8403d1284007e4f18227c3c`  
		Last Modified: Sat, 26 Sep 2020 00:07:35 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a325c5e893eb9c1eee88bc23abc49cb3bd3981f0ad75bc13f858ceef122813d`  
		Last Modified: Sat, 26 Sep 2020 00:07:40 GMT  
		Size: 17.7 MB (17693393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03255d53b60da941950d8ba5851576b778efc2e7c2cc8226f619ba710c2c71c`  
		Last Modified: Sat, 26 Sep 2020 00:07:34 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aedc819f3a24e1c512e9bd88ba7fe3534e2825040017f12962240208308ee1`  
		Last Modified: Sat, 26 Sep 2020 00:07:34 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbccf79a85ad8d68e31983400cf9cdb914b809b9fbf8af979bb630bd8fb734f`  
		Last Modified: Sat, 26 Sep 2020 00:07:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0347ef53e57ae098b9720a743c36081805b1c00154ce5516b5e1722b31ce7db3`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4366217d729e94916c5bc4f011e863c4436a4f0e28e4aaa7dd38003881c8bfe4`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801beab1a0fa531e11c5c71fe5f9f56f943dd6fef67da4a8816e89deff12a6ef`  
		Last Modified: Sat, 26 Sep 2020 00:07:32 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b7e1df959ce557740ad55e730b687d45931b310c51b9e7163fa43e289c45f`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765ffe959a7df80c92bc3945ac720d3f343f230085dd6c8f112277977b97fcc`  
		Last Modified: Sat, 26 Sep 2020 00:07:30 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7299920606443a615204b88ae0b26d76f566ae80edb84a43420e971ab8279`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfff45371f5fa6f168f03bf11bbb1f1d751d56c056a3b839aec270c6b276d74`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758bdbc1a34c4a22c92f52b973388589243178ed62087eede3079f411b8dd061`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb7fb0b899cafbd14fde4f7903c37dd72bdf91a0444cce9da878c29d80027ac`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62de917f277d9dd32c53e7132b66397808f4a1db49da287b123f906e3956c2eb`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ceef103e926f07af4c4d9419212cf30c0e8fa54adb173e4eb4713d2a01563e`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe48c00ec807e1297e9bb0011a8223135ae2228a413fd77bc6ed8075d842f6`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac963d0f2ed9ce1bae553fa884a12c187e56d3b5f15ffb00e7a5472c667be73`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 306.2 KB (306189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087f889bde7ffdb3305c8da1fa9e5474b8bf585fb276ad612928d92f3bcb1ff7`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:3eaa72122a1c8777eebb9cb70237412d32f5d00d61deb258a7297dcc01a3915e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772324795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44bcb3197a91f6005135d9d64c534684de99522992a8b00ab5a4b53084889c1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:23:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:23:45 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:25:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:25:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:25:11 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:25:12 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 22:25:13 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 22:25:14 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:25:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:25:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:25:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:25:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:25:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:25:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:25:19 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:25:19 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:25:20 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:26:03 GMT
RUN caddy version
# Fri, 25 Sep 2020 22:26:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d72b7607b806beed4aafbaccee5c30d613fa762498a797c526cef45222ec10`  
		Last Modified: Sat, 26 Sep 2020 00:08:01 GMT  
		Size: 9.9 MB (9905052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731e7579ab3965dda5a9e41c556c4ca32ccdae9be5ec6e7f46bd647f1fe63891`  
		Last Modified: Sat, 26 Sep 2020 00:07:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fff091c5777968177457a4e9c3aadc893e97f676d024ff5d237158f6c11da7a`  
		Last Modified: Sat, 26 Sep 2020 00:08:02 GMT  
		Size: 22.9 MB (22883540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d05a19446e8af754abceeb85b4631270875c30039d1c3b18a2be62a87fa8c31`  
		Last Modified: Sat, 26 Sep 2020 00:07:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a81327f32b6df82f48e52941f7c74fc59329d2c2d19cb7e67ad728e1bde546`  
		Last Modified: Sat, 26 Sep 2020 00:07:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507b4bf1c0aeb5d728e5277920623c8cb340b2e022f0c2b1e4f56e48528325c6`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b499a6f00e79ce856374f971408bbef25bacc81b012dbd23d2a029397de8238`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92048406361df5dd644d39ff147bc808ada0abdbc5be7589ce6acc74cb806bb9`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b3fb321d9fd8cc3646329da5b16664e63a57f8103630ff5d0fdb9aa55eb704`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8c4aa6d8ea1a517610a94bbc5e569df76d6e4a4b4848094972f3434e750472`  
		Last Modified: Sat, 26 Sep 2020 00:07:52 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c6d9999d1602c8dd10d24038cb7a853fa7675166e2574c22194e21b089f98e`  
		Last Modified: Sat, 26 Sep 2020 00:07:51 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3af868fe329ff3ec48e457c9cb6cf7f6db59ad6d496ad21a9d085ac4c9866e`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97187facc53e9385bbd1faf9f94eec9fd67187acb185b241c342356adec229a`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebb7ad698eeacf880cb61aabb841a2f3fd67885737916aef11b9b6508033594`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b28bc94f5ccc03dc1591e017f819c2b10d6e481b3bee66604e609ae71b449b3`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f091e541c5f573cc9bf8b6d3427495211b798bfb620353216667bd80478ed`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf2458da5062b0b24b86e9f69a30538248926ad9e2b8411d32e5955cb67fe3`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25600a431dfe7d2457a4223132df9f335cc891853d4623583f55f16adfe1760a`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2e4ecbae8bfa668a1e0ff5815f029a57708a6c20c764c77a6a574839eefb82`  
		Last Modified: Sat, 26 Sep 2020 00:07:48 GMT  
		Size: 261.4 KB (261429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f7c356a4c3f5ed1e8c67b8c3832a05e5f651cbbd20f19dda4ee676e779b80f`  
		Last Modified: Sat, 26 Sep 2020 00:07:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-alpine`

```console
$ docker pull caddy@sha256:0423525df39f98ebbdaa054439fb4b51a650f0da9af188f681f696bad64c095e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:80d608bfebf1d919d7613d401af6004ba74a3be96867e1a25d9ab35a2da6714f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fd8ade3df48988e09df79afd3361daa868169892daa8efc4b9b88028fada48a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:27:13 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:27:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:16 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:16 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:17 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:18 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:18 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:19 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:19 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff8cd7408716264fcaa599bf31e94490e2cf2281ce3d87c7376ecaabf995f2c`  
		Last Modified: Fri, 25 Sep 2020 22:27:59 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445f33e99ec338357aded23d1cf928a75a2ce5f6c840c49fc4a9469c0de07700`  
		Last Modified: Fri, 25 Sep 2020 22:28:01 GMT  
		Size: 13.1 MB (13057337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2107641907cbbc1ab9d5f92fc706779dfb06fa4f287e29f0e0731d27efab1d`  
		Last Modified: Fri, 25 Sep 2020 22:27:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6a6e8e419c6b07de12627d56e57d7526bbf0b7e0ed6444059310741aa823bf85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32588090d7bb2509380b4739113c43093f60dba0016465ed03143ef0225790e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:49:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:49:30 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:49:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:49:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:49:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:49:38 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:49:39 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:49:39 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:49:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:49:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:49:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:49:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:49:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:49:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:49:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:49:45 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:49:46 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:49:46 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:49:47 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f230a7df78269514af68ed5207d0d2ade5646619012a49f07564abd097a4f43`  
		Last Modified: Fri, 25 Sep 2020 22:51:00 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9826d83e7a201860c01ef0c6b537b3c7b672a109e04dc5e37b58051a7173ec21`  
		Last Modified: Fri, 25 Sep 2020 22:51:05 GMT  
		Size: 12.4 MB (12414930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20425603e5d968a6603537e218e4cc64a53b97498cbaf265bd952b931f6bbea`  
		Last Modified: Fri, 25 Sep 2020 22:51:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b1d5c01fc7bfacc51f7d10dcdcb0b6b8de3aac2df9bfd8db586d207d88f2a833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a694089ff1fc1cffa1e5ea27b0ae3f3cf3c40ee1d21bcf6e9eb7ea94352b4fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:57:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:57:50 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:57:58 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:57:59 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:57:59 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:58:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:07 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:08 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c815fe644041cd1e2a8be930b155833108c9af6b9214feb5b1c2f3b1710842af`  
		Last Modified: Fri, 25 Sep 2020 22:59:26 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c03433041ed8c869ebfd10d91d6673d1892324cbad0cdf2bdfb7eedc084a9d`  
		Last Modified: Fri, 25 Sep 2020 22:59:30 GMT  
		Size: 12.4 MB (12396043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8766336719d6750ac25a3c3bb665a18388a58138b4cdf8792ffc8aeb49c0099f`  
		Last Modified: Fri, 25 Sep 2020 22:59:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:04c78db76cedc0f3b4c2133fdc640dd69b1d9899b74b006c122f18352ab5fb1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe2123125accfb26638d3d060043f8032c66ff423f24993e350219facbf429c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:39:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:39:36 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:39:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:39:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:39:42 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:39:43 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:39:43 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:39:44 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:39:45 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:39:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:39:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:39:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:39:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:39:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:39:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:39:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:39:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:39:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:39:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:39:52 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:39:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7ce2e195b05936e35a055c73bad445ca921206fd8c0c018f8a9b882488ec1a`  
		Last Modified: Fri, 25 Sep 2020 22:41:07 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0170c97deb56c282ca48bf564346008e7f0e44767d6e54a3cc25403771f36957`  
		Last Modified: Fri, 25 Sep 2020 22:41:10 GMT  
		Size: 12.0 MB (12013100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f581aff5bd1747039f52bd705bbe5482b368537c82ea8d9ec22c966a97dbc`  
		Last Modified: Fri, 25 Sep 2020 22:41:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d5fc341e5909164e6d09c5aa91ffea06ecdec40e4ece378e4d20a05ca1ac2d38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67135043576dd821b2eebd66491f6bdf03d306dd63f80ae70348a3a44d12f63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:34:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:34:28 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:34:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:35:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:35:08 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:35:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:35:37 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:35:49 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:36:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:36:18 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:36:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:36:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:36:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:36:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:37:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:37:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:37:29 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:37:41 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:37:56 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:38:09 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:38:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c2cc7761fc2675da80a24060fc865587f2c860a62a474056465c2402d691f8`  
		Last Modified: Fri, 25 Sep 2020 22:45:07 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98625f8d1b9c837094e190b29036054a427daabf5d3945434b54c89da129cc43`  
		Last Modified: Fri, 25 Sep 2020 22:45:10 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca513b6513d2e7c22c90baf1a8509f6d91cfc20edb99506d72239f7e755d62d`  
		Last Modified: Fri, 25 Sep 2020 22:45:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:20408b3f483d7f32960f3839286b404f633ae99da1e8932dc429bc0c6b3a94b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84cdf8e8f810203a97d0597b2d9f5bab7d5b0eecb14ed3a12237bdea870bf2c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"
# Fri, 25 Sep 2020 22:41:22 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:41:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:26 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:26 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:27 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:27 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:41:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:29 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:29 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:29 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:29 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13489b412dcfe7f996349c0742c4bbefde864c19defb8240fa21a95881ea436`  
		Last Modified: Fri, 25 Sep 2020 22:42:11 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe4b720629eafad7b4379d0af34dcfd8d8de2540c694d2e1f420f89b2ee5d68`  
		Last Modified: Fri, 25 Sep 2020 22:42:13 GMT  
		Size: 12.8 MB (12836819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873125611edecc47abc85437ff79cdbf0c56c9d7509ac7e7a3941f87323e9fa4`  
		Last Modified: Fri, 25 Sep 2020 22:42:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder`

```console
$ docker pull caddy@sha256:5a6e9207f25c6cef30830c7586dae2971b82b94d763b8a7a8d305304c336f69b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.1.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:d5f7999af933a6d3350e575786a2f16aba5e930513faa770602b0e4bff23f1f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120169717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9523c15dba19a965a9876feb739c5e803195ef8873e9e1717cec30807013bfff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:58 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:25:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:25:12 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:25:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:25:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:25:13 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:25 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:25 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:27:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0547b08c8963faeee9d579d8351699f769179aa7a58ada0290e6ab8f5a676c`  
		Last Modified: Wed, 09 Sep 2020 22:30:12 GMT  
		Size: 107.4 MB (107371657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b6f0657434294654385190364b1a7c9af2a6f7b7ef0e821b8d51e20cdd8da5`  
		Last Modified: Wed, 09 Sep 2020 22:29:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b6567fb8ec7e0ec3b0ae6600ccda0528e94ef892ebb7437d9a3d2618e52d2c`  
		Last Modified: Fri, 25 Sep 2020 22:28:06 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea9a80e0e2435373930ec1446faf55a0c9a6c38c6345c8dc311f53980bea9cc`  
		Last Modified: Fri, 25 Sep 2020 22:28:05 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca5e78208a09f95566cee8aaf87377d4a90ee0876ed6cfef4112094985eafc`  
		Last Modified: Fri, 25 Sep 2020 22:28:04 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a8307a5e8bbafa996de097f1ce5cce7356ca69dd876f73b75c81981d070e271f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115855840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ccc058ff7d3bdf7ba573fd105e819d1b549cee1155c15878e62d4ddc3183d6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:54:15 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:57:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:57:19 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:57:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:57:23 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:49:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:49:58 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:49:59 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:49:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6fe6c5f0fa89cff72714190eb250d37035e32c7216624ea20cfcdfc88d8932`  
		Last Modified: Wed, 09 Sep 2020 23:02:32 GMT  
		Size: 103.7 MB (103712873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186bd058112580f710efc27a0aae302bc22b6933011ca92545db5a513ddde4c0`  
		Last Modified: Wed, 09 Sep 2020 23:02:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabce2f857cbac8727f8021a5cf32f58d584d215c2e8335b66f0219a29a3033d`  
		Last Modified: Fri, 25 Sep 2020 22:51:13 GMT  
		Size: 7.9 MB (7928840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e241c148840303273064a679499c21f3aca20b4aaf58c77f28779e279fb48f84`  
		Last Modified: Fri, 25 Sep 2020 22:51:11 GMT  
		Size: 1.3 MB (1327350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27b1b507797e2939000db251e060bed35635884911e1ca2169971fffcc486b2`  
		Last Modified: Fri, 25 Sep 2020 22:51:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f67a650b90e8d2a154c1c2b336cfe21520f944706539151c61f3afaee7793d4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114622952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3abcefdc9bf61ec46fb1d63b3460e4632f700d7557c697007c9eed2efa0d826`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:05:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:07:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:07:51 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:07:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:07:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:07:54 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:58:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:58:19 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:58:20 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:58:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:58:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:58:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:58:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189358c25ed3947ca4fd93936880bae2e9a32a62f75d865d03db0ce536130f63`  
		Last Modified: Wed, 09 Sep 2020 22:14:22 GMT  
		Size: 103.5 MB (103462777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a5f301bfa0a4263c5e4fd043d781161d2579b6d5ac42d3a18287f1452e4194`  
		Last Modified: Wed, 09 Sep 2020 22:13:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66072234449cb7ebdfa002c42bc8bc4d2bd9b9fc3eb35b2f42f97cda16e9c465`  
		Last Modified: Fri, 25 Sep 2020 22:59:37 GMT  
		Size: 7.1 MB (7144963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057878579f01640f17bd812b5eb955522f4417c13140581f324bd45ec72c8171`  
		Last Modified: Fri, 25 Sep 2020 22:59:36 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f2dd8c431593bb818262a0f6cf4e99384b7a3bd428eaf77e41adcdd56d1b61`  
		Last Modified: Fri, 25 Sep 2020 22:59:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ae0a341e115b71cabe57716540ed3f37cc4a8781968014872b092cc4056dcc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115613481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d8bff2d69027fa736b15d37f3bd4a0d25526f3a5ba62d9e5fc9edddee2a7ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:22 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:10 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:14 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:40:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee363a75d12710f67004978ba4509d1ddb769cc47ba518bc277ecd103a6b8d`  
		Last Modified: Wed, 09 Sep 2020 22:51:01 GMT  
		Size: 102.8 MB (102811724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab2d6f42095309ce47a6ec4edd38bd86aabe0fb28a18cb007652d42e0f19e0`  
		Last Modified: Wed, 09 Sep 2020 22:50:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3daf327048ea4a763cbf539c90940c6b9aa38c855f7ef3ed94cd8ec78b3f0`  
		Last Modified: Fri, 25 Sep 2020 22:41:18 GMT  
		Size: 8.5 MB (8499903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060cae146f34b58e867a469646d5890b88814e89f40e79bf189a0d8328794bf3`  
		Last Modified: Fri, 25 Sep 2020 22:41:16 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e04b02068c1b0c55346de19ab65cfaf81f0c7e592e3b9186770805d808cc2f`  
		Last Modified: Fri, 25 Sep 2020 22:41:16 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:123d4d4d278526a8e701cd04340f1dba7b30e30c5c5670eb1262a135c5b10cd8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114975359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353c0018d03b3c5caaf56597dad9f71994ee3484891dafa93293c87c52e89970`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:26:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:29:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:29:52 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:29:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:30:39 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:38:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:39:05 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:39:17 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:39:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:39:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:39:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:02 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba569e5c85b1b70b3985f097dd79fee89c81c111899c623098e368323e560524`  
		Last Modified: Wed, 09 Sep 2020 22:44:05 GMT  
		Size: 101.7 MB (101676592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cb177af69484b6f3437a2174165ac7a6c677d76f72e742f049397fb1fe2df`  
		Last Modified: Wed, 09 Sep 2020 22:43:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b9f0d89c6dc27e3c5c140b29344ef655160fc9e88f4196c49fe8dc1ed7e920`  
		Last Modified: Fri, 25 Sep 2020 22:45:22 GMT  
		Size: 8.9 MB (8920029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb48f7a86e8728bdc83e425192be427270c4373d75021b798b6d823187d98c0`  
		Last Modified: Fri, 25 Sep 2020 22:45:20 GMT  
		Size: 1.3 MB (1287790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e11ed799593484a68e98ebebc5a412185deced61c2a18bc4c822c534533ae69`  
		Last Modified: Fri, 25 Sep 2020 22:45:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1285082a295430e40664f8c45d9afaeef9882396aee2a9032e0148419bd1815e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119845154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e8e2ac6196cf2f55081248aa3fa9679367f116d18ae3d94f928bbdd1979a38`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:55 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:07 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:08 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:36 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:36 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e7f0b644229c4d22243efaf9cde7728d52c4624e9d48ab2d5174ec187de5f9`  
		Last Modified: Wed, 09 Sep 2020 22:48:16 GMT  
		Size: 107.3 MB (107254107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b1ab98332292b26f0fee8484fc91221c2e937011cbcd0fa39c2b7f8b32252e`  
		Last Modified: Wed, 09 Sep 2020 22:48:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3410d79dc81d3365abcfd9af5b2a59c63ca9271245267f755bd050b16b7e223e`  
		Last Modified: Fri, 25 Sep 2020 22:42:19 GMT  
		Size: 8.4 MB (8352248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65b31e4bcee38a9106ed828122ca5dbf26b0eb949b75812a7cef4030e433b28`  
		Last Modified: Fri, 25 Sep 2020 22:42:18 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e19ef40a33a5b2d606204c7a107998bb8d08dbf01e36c3a3bfaee4ec4d46b8`  
		Last Modified: Fri, 25 Sep 2020 22:42:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:ff54e1d18a4188ebb0c348f7d6f5214973b0a795fb527acba93f5808ad751b43
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2529791101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:318045548d0cc0a5d58d9a7de72dfa6ab6e5f9cb7ab497ee79a7c37e9e99fb36`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:24:50 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:27:29 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '16bb44448c4423740c5fd751bad28061d5ec44cd08272d4e1efdd16cdf8221e9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:27:31 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 22:26:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:26:11 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:26:12 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:26:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:56:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 25 Sep 2020 22:56:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14e699fd824b87316986d5a6510231d15eb3df99fc1e784d00d550f70e6d9fd`  
		Last Modified: Wed, 09 Sep 2020 22:37:05 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be2a93ed64b5c58235e6b05e350584bb558e6434aafec38e553cf76b8568e0b`  
		Last Modified: Wed, 09 Sep 2020 22:37:31 GMT  
		Size: 137.8 MB (137834948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61553c8eaef2c4d92699812e4508d392ef255f8966edc3eb78c96cad58036a7d`  
		Last Modified: Wed, 09 Sep 2020 22:37:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07c69a11ed365247b6d6b659c1be89cc3bfa5792f938682a296843cd4d5c436`  
		Last Modified: Sat, 26 Sep 2020 00:08:12 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e03ec02f675645b2ac5f6e2399be5fa7aa74102ee959bde5fadc7ecf5b4e4`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71b5ece697ba3e27ad157522ee683991a67156fa39f6686ef166fb26a2eb4ea`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865184d2df3e1d10dcc5991108b8f9e58de0420a46b612f0a8a6b79934f859e2`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d10df838c70a675f668567354ea6717573aa4e17fdfa70a07d38520ddce5f`  
		Last Modified: Sat, 26 Sep 2020 00:08:13 GMT  
		Size: 6.2 MB (6151041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b98afae2235ace15abdc761a3909090f4fba392af8843a23c46311821ac751`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:195eed51b16dc9dce08177c5fccc02b920049dbf2c138b30a60c6e0cd715b74d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5933926837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595a7b5205de69e08d581fbfa113c23fbe75019624b5f9ba775eb1e2a8ba61f0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:27:46 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:31:15 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '16bb44448c4423740c5fd751bad28061d5ec44cd08272d4e1efdd16cdf8221e9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:31:16 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 22:57:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:57:01 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:57:02 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:58:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 25 Sep 2020 22:58:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12afd1ebb298a520d1e78b3dc0f3cee23655d646c655fe01118d22c1a380d85c`  
		Last Modified: Wed, 09 Sep 2020 22:37:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb28d852e2d4f73640ef6d741c833810c410bcfa3b80faec19526a5fc16e900`  
		Last Modified: Wed, 09 Sep 2020 22:40:21 GMT  
		Size: 143.0 MB (143009844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b770fdb51315fdfd8cd507559384c304c74c9352af52dab72a53329e1e1867`  
		Last Modified: Wed, 09 Sep 2020 22:37:42 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c82fbbebbec334f8e6311b9a45fb48ef29f01eed5a14a6cafa283c9c3c80426`  
		Last Modified: Sat, 26 Sep 2020 00:08:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850b0bf35c5a647c01ce9a04f299e946ddde56f2957bb6ec478c8eed550d3589`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8347bd99966020ba60cbb4615cef2c98a12634b4b8dec47f3665dcc30f3bfc6d`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dbd08bf9634ff1677a8ba8aefabaab0b6bde008410a1568989f15bb9c214b6`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20cb08a2cdc84f87975be6ddd3d8f1fc7a1e23d8f16c4d9ce4bb39c02d4d8fb`  
		Last Modified: Sat, 26 Sep 2020 00:08:26 GMT  
		Size: 11.3 MB (11321037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7835dc239ce73c485f908234d3582554a1371af4ededf7a608d4715814ef48d`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-alpine`

```console
$ docker pull caddy@sha256:589f69d3b427997c0d1091068c65d8e57424cc7e77674c4137c26552d6bd0410
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:d5f7999af933a6d3350e575786a2f16aba5e930513faa770602b0e4bff23f1f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120169717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9523c15dba19a965a9876feb739c5e803195ef8873e9e1717cec30807013bfff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:58 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:25:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:25:12 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:25:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:25:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:25:13 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:25 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:25 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:27:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:27 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0547b08c8963faeee9d579d8351699f769179aa7a58ada0290e6ab8f5a676c`  
		Last Modified: Wed, 09 Sep 2020 22:30:12 GMT  
		Size: 107.4 MB (107371657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b6f0657434294654385190364b1a7c9af2a6f7b7ef0e821b8d51e20cdd8da5`  
		Last Modified: Wed, 09 Sep 2020 22:29:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b6567fb8ec7e0ec3b0ae6600ccda0528e94ef892ebb7437d9a3d2618e52d2c`  
		Last Modified: Fri, 25 Sep 2020 22:28:06 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea9a80e0e2435373930ec1446faf55a0c9a6c38c6345c8dc311f53980bea9cc`  
		Last Modified: Fri, 25 Sep 2020 22:28:05 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca5e78208a09f95566cee8aaf87377d4a90ee0876ed6cfef4112094985eafc`  
		Last Modified: Fri, 25 Sep 2020 22:28:04 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a8307a5e8bbafa996de097f1ce5cce7356ca69dd876f73b75c81981d070e271f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115855840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ccc058ff7d3bdf7ba573fd105e819d1b549cee1155c15878e62d4ddc3183d6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:54:15 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:57:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:57:19 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:57:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:57:23 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:49:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:49:58 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:49:59 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:49:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6fe6c5f0fa89cff72714190eb250d37035e32c7216624ea20cfcdfc88d8932`  
		Last Modified: Wed, 09 Sep 2020 23:02:32 GMT  
		Size: 103.7 MB (103712873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186bd058112580f710efc27a0aae302bc22b6933011ca92545db5a513ddde4c0`  
		Last Modified: Wed, 09 Sep 2020 23:02:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabce2f857cbac8727f8021a5cf32f58d584d215c2e8335b66f0219a29a3033d`  
		Last Modified: Fri, 25 Sep 2020 22:51:13 GMT  
		Size: 7.9 MB (7928840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e241c148840303273064a679499c21f3aca20b4aaf58c77f28779e279fb48f84`  
		Last Modified: Fri, 25 Sep 2020 22:51:11 GMT  
		Size: 1.3 MB (1327350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27b1b507797e2939000db251e060bed35635884911e1ca2169971fffcc486b2`  
		Last Modified: Fri, 25 Sep 2020 22:51:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f67a650b90e8d2a154c1c2b336cfe21520f944706539151c61f3afaee7793d4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114622952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3abcefdc9bf61ec46fb1d63b3460e4632f700d7557c697007c9eed2efa0d826`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:05:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:07:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:07:51 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:07:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:07:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:07:54 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:58:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:58:19 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:58:20 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:58:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:58:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:58:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:58:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189358c25ed3947ca4fd93936880bae2e9a32a62f75d865d03db0ce536130f63`  
		Last Modified: Wed, 09 Sep 2020 22:14:22 GMT  
		Size: 103.5 MB (103462777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a5f301bfa0a4263c5e4fd043d781161d2579b6d5ac42d3a18287f1452e4194`  
		Last Modified: Wed, 09 Sep 2020 22:13:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66072234449cb7ebdfa002c42bc8bc4d2bd9b9fc3eb35b2f42f97cda16e9c465`  
		Last Modified: Fri, 25 Sep 2020 22:59:37 GMT  
		Size: 7.1 MB (7144963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057878579f01640f17bd812b5eb955522f4417c13140581f324bd45ec72c8171`  
		Last Modified: Fri, 25 Sep 2020 22:59:36 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f2dd8c431593bb818262a0f6cf4e99384b7a3bd428eaf77e41adcdd56d1b61`  
		Last Modified: Fri, 25 Sep 2020 22:59:36 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ae0a341e115b71cabe57716540ed3f37cc4a8781968014872b092cc4056dcc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115613481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d8bff2d69027fa736b15d37f3bd4a0d25526f3a5ba62d9e5fc9edddee2a7ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:22 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:10 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:14 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:03 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:05 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:40:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee363a75d12710f67004978ba4509d1ddb769cc47ba518bc277ecd103a6b8d`  
		Last Modified: Wed, 09 Sep 2020 22:51:01 GMT  
		Size: 102.8 MB (102811724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab2d6f42095309ce47a6ec4edd38bd86aabe0fb28a18cb007652d42e0f19e0`  
		Last Modified: Wed, 09 Sep 2020 22:50:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3daf327048ea4a763cbf539c90940c6b9aa38c855f7ef3ed94cd8ec78b3f0`  
		Last Modified: Fri, 25 Sep 2020 22:41:18 GMT  
		Size: 8.5 MB (8499903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060cae146f34b58e867a469646d5890b88814e89f40e79bf189a0d8328794bf3`  
		Last Modified: Fri, 25 Sep 2020 22:41:16 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e04b02068c1b0c55346de19ab65cfaf81f0c7e592e3b9186770805d808cc2f`  
		Last Modified: Fri, 25 Sep 2020 22:41:16 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:123d4d4d278526a8e701cd04340f1dba7b30e30c5c5670eb1262a135c5b10cd8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (114975359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353c0018d03b3c5caaf56597dad9f71994ee3484891dafa93293c87c52e89970`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:26:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:29:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:29:52 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:29:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:30:39 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:38:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:39:05 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:39:17 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:39:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:39:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:39:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:02 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba569e5c85b1b70b3985f097dd79fee89c81c111899c623098e368323e560524`  
		Last Modified: Wed, 09 Sep 2020 22:44:05 GMT  
		Size: 101.7 MB (101676592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cb177af69484b6f3437a2174165ac7a6c677d76f72e742f049397fb1fe2df`  
		Last Modified: Wed, 09 Sep 2020 22:43:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b9f0d89c6dc27e3c5c140b29344ef655160fc9e88f4196c49fe8dc1ed7e920`  
		Last Modified: Fri, 25 Sep 2020 22:45:22 GMT  
		Size: 8.9 MB (8920029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb48f7a86e8728bdc83e425192be427270c4373d75021b798b6d823187d98c0`  
		Last Modified: Fri, 25 Sep 2020 22:45:20 GMT  
		Size: 1.3 MB (1287790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e11ed799593484a68e98ebebc5a412185deced61c2a18bc4c822c534533ae69`  
		Last Modified: Fri, 25 Sep 2020 22:45:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:1285082a295430e40664f8c45d9afaeef9882396aee2a9032e0148419bd1815e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119845154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e8e2ac6196cf2f55081248aa3fa9679367f116d18ae3d94f928bbdd1979a38`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:55 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:07 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:08 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:36 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:36 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:41:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e7f0b644229c4d22243efaf9cde7728d52c4624e9d48ab2d5174ec187de5f9`  
		Last Modified: Wed, 09 Sep 2020 22:48:16 GMT  
		Size: 107.3 MB (107254107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b1ab98332292b26f0fee8484fc91221c2e937011cbcd0fa39c2b7f8b32252e`  
		Last Modified: Wed, 09 Sep 2020 22:48:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3410d79dc81d3365abcfd9af5b2a59c63ca9271245267f755bd050b16b7e223e`  
		Last Modified: Fri, 25 Sep 2020 22:42:19 GMT  
		Size: 8.4 MB (8352248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65b31e4bcee38a9106ed828122ca5dbf26b0eb949b75812a7cef4030e433b28`  
		Last Modified: Fri, 25 Sep 2020 22:42:18 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e19ef40a33a5b2d606204c7a107998bb8d08dbf01e36c3a3bfaee4ec4d46b8`  
		Last Modified: Fri, 25 Sep 2020 22:42:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f7822640dff5384830b18c91624912af1b77483997ed159d15db5db74c0fc33e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2.1.1-builder-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:ff54e1d18a4188ebb0c348f7d6f5214973b0a795fb527acba93f5808ad751b43
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2529791101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:318045548d0cc0a5d58d9a7de72dfa6ab6e5f9cb7ab497ee79a7c37e9e99fb36`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:24:50 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:27:29 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '16bb44448c4423740c5fd751bad28061d5ec44cd08272d4e1efdd16cdf8221e9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:27:31 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 22:26:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:26:11 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:26:12 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:26:12 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:56:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 25 Sep 2020 22:56:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14e699fd824b87316986d5a6510231d15eb3df99fc1e784d00d550f70e6d9fd`  
		Last Modified: Wed, 09 Sep 2020 22:37:05 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be2a93ed64b5c58235e6b05e350584bb558e6434aafec38e553cf76b8568e0b`  
		Last Modified: Wed, 09 Sep 2020 22:37:31 GMT  
		Size: 137.8 MB (137834948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61553c8eaef2c4d92699812e4508d392ef255f8966edc3eb78c96cad58036a7d`  
		Last Modified: Wed, 09 Sep 2020 22:37:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07c69a11ed365247b6d6b659c1be89cc3bfa5792f938682a296843cd4d5c436`  
		Last Modified: Sat, 26 Sep 2020 00:08:12 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e03ec02f675645b2ac5f6e2399be5fa7aa74102ee959bde5fadc7ecf5b4e4`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71b5ece697ba3e27ad157522ee683991a67156fa39f6686ef166fb26a2eb4ea`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865184d2df3e1d10dcc5991108b8f9e58de0420a46b612f0a8a6b79934f859e2`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d10df838c70a675f668567354ea6717573aa4e17fdfa70a07d38520ddce5f`  
		Last Modified: Sat, 26 Sep 2020 00:08:13 GMT  
		Size: 6.2 MB (6151041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b98afae2235ace15abdc761a3909090f4fba392af8843a23c46311821ac751`  
		Last Modified: Sat, 26 Sep 2020 00:08:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:117871610aebf4663cf46f53bef8939d00ba520bb1304e099f1957e5b88a488b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.1.1-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:195eed51b16dc9dce08177c5fccc02b920049dbf2c138b30a60c6e0cd715b74d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5933926837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595a7b5205de69e08d581fbfa113c23fbe75019624b5f9ba775eb1e2a8ba61f0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:27:46 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:31:15 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.14.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '16bb44448c4423740c5fd751bad28061d5ec44cd08272d4e1efdd16cdf8221e9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:31:16 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 22:57:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:57:01 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:57:02 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:58:24 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Fri, 25 Sep 2020 22:58:25 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12afd1ebb298a520d1e78b3dc0f3cee23655d646c655fe01118d22c1a380d85c`  
		Last Modified: Wed, 09 Sep 2020 22:37:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb28d852e2d4f73640ef6d741c833810c410bcfa3b80faec19526a5fc16e900`  
		Last Modified: Wed, 09 Sep 2020 22:40:21 GMT  
		Size: 143.0 MB (143009844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b770fdb51315fdfd8cd507559384c304c74c9352af52dab72a53329e1e1867`  
		Last Modified: Wed, 09 Sep 2020 22:37:42 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c82fbbebbec334f8e6311b9a45fb48ef29f01eed5a14a6cafa283c9c3c80426`  
		Last Modified: Sat, 26 Sep 2020 00:08:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850b0bf35c5a647c01ce9a04f299e946ddde56f2957bb6ec478c8eed550d3589`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8347bd99966020ba60cbb4615cef2c98a12634b4b8dec47f3665dcc30f3bfc6d`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dbd08bf9634ff1677a8ba8aefabaab0b6bde008410a1568989f15bb9c214b6`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20cb08a2cdc84f87975be6ddd3d8f1fc7a1e23d8f16c4d9ce4bb39c02d4d8fb`  
		Last Modified: Sat, 26 Sep 2020 00:08:26 GMT  
		Size: 11.3 MB (11321037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7835dc239ce73c485f908234d3582554a1371af4ededf7a608d4715814ef48d`  
		Last Modified: Sat, 26 Sep 2020 00:08:23 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore`

```console
$ docker pull caddy@sha256:43d894e170267ba73034945c16b270807496de1f87bb313b200d3b1c9835b7a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.1.1-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:0c81e39f253977e239df5f59cf89da2f5c7f009ce1dab3af9c935b96ace5f111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378453354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b788438493f88710ba4198f5a8e2324ba21a891ac37ad2d9279608278dae239e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:21:26 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:21:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:21:59 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:22:00 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:22:01 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 22:22:01 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 22:22:02 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:22:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:22:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:22:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:22:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:22:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:22:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:22:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:22:07 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:22:08 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:22:09 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:22:23 GMT
RUN caddy version
# Fri, 25 Sep 2020 22:22:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a93d915a3d15febf5cb14d3ce13f84e4e1b59e54251670dffff8c859031c10a`  
		Last Modified: Sat, 26 Sep 2020 00:07:38 GMT  
		Size: 9.2 MB (9161113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af424f647689600c8a89cb1e4745cfc5f8a9ec3fa8403d1284007e4f18227c3c`  
		Last Modified: Sat, 26 Sep 2020 00:07:35 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a325c5e893eb9c1eee88bc23abc49cb3bd3981f0ad75bc13f858ceef122813d`  
		Last Modified: Sat, 26 Sep 2020 00:07:40 GMT  
		Size: 17.7 MB (17693393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03255d53b60da941950d8ba5851576b778efc2e7c2cc8226f619ba710c2c71c`  
		Last Modified: Sat, 26 Sep 2020 00:07:34 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aedc819f3a24e1c512e9bd88ba7fe3534e2825040017f12962240208308ee1`  
		Last Modified: Sat, 26 Sep 2020 00:07:34 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbccf79a85ad8d68e31983400cf9cdb914b809b9fbf8af979bb630bd8fb734f`  
		Last Modified: Sat, 26 Sep 2020 00:07:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0347ef53e57ae098b9720a743c36081805b1c00154ce5516b5e1722b31ce7db3`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4366217d729e94916c5bc4f011e863c4436a4f0e28e4aaa7dd38003881c8bfe4`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801beab1a0fa531e11c5c71fe5f9f56f943dd6fef67da4a8816e89deff12a6ef`  
		Last Modified: Sat, 26 Sep 2020 00:07:32 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b7e1df959ce557740ad55e730b687d45931b310c51b9e7163fa43e289c45f`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765ffe959a7df80c92bc3945ac720d3f343f230085dd6c8f112277977b97fcc`  
		Last Modified: Sat, 26 Sep 2020 00:07:30 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7299920606443a615204b88ae0b26d76f566ae80edb84a43420e971ab8279`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfff45371f5fa6f168f03bf11bbb1f1d751d56c056a3b839aec270c6b276d74`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758bdbc1a34c4a22c92f52b973388589243178ed62087eede3079f411b8dd061`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb7fb0b899cafbd14fde4f7903c37dd72bdf91a0444cce9da878c29d80027ac`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62de917f277d9dd32c53e7132b66397808f4a1db49da287b123f906e3956c2eb`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ceef103e926f07af4c4d9419212cf30c0e8fa54adb173e4eb4713d2a01563e`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe48c00ec807e1297e9bb0011a8223135ae2228a413fd77bc6ed8075d842f6`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac963d0f2ed9ce1bae553fa884a12c187e56d3b5f15ffb00e7a5472c667be73`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 306.2 KB (306189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087f889bde7ffdb3305c8da1fa9e5474b8bf585fb276ad612928d92f3bcb1ff7`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:3eaa72122a1c8777eebb9cb70237412d32f5d00d61deb258a7297dcc01a3915e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772324795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44bcb3197a91f6005135d9d64c534684de99522992a8b00ab5a4b53084889c1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:23:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:23:45 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:25:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:25:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:25:11 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:25:12 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 22:25:13 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 22:25:14 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:25:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:25:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:25:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:25:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:25:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:25:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:25:19 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:25:19 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:25:20 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:26:03 GMT
RUN caddy version
# Fri, 25 Sep 2020 22:26:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d72b7607b806beed4aafbaccee5c30d613fa762498a797c526cef45222ec10`  
		Last Modified: Sat, 26 Sep 2020 00:08:01 GMT  
		Size: 9.9 MB (9905052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731e7579ab3965dda5a9e41c556c4ca32ccdae9be5ec6e7f46bd647f1fe63891`  
		Last Modified: Sat, 26 Sep 2020 00:07:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fff091c5777968177457a4e9c3aadc893e97f676d024ff5d237158f6c11da7a`  
		Last Modified: Sat, 26 Sep 2020 00:08:02 GMT  
		Size: 22.9 MB (22883540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d05a19446e8af754abceeb85b4631270875c30039d1c3b18a2be62a87fa8c31`  
		Last Modified: Sat, 26 Sep 2020 00:07:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a81327f32b6df82f48e52941f7c74fc59329d2c2d19cb7e67ad728e1bde546`  
		Last Modified: Sat, 26 Sep 2020 00:07:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507b4bf1c0aeb5d728e5277920623c8cb340b2e022f0c2b1e4f56e48528325c6`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b499a6f00e79ce856374f971408bbef25bacc81b012dbd23d2a029397de8238`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92048406361df5dd644d39ff147bc808ada0abdbc5be7589ce6acc74cb806bb9`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b3fb321d9fd8cc3646329da5b16664e63a57f8103630ff5d0fdb9aa55eb704`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8c4aa6d8ea1a517610a94bbc5e569df76d6e4a4b4848094972f3434e750472`  
		Last Modified: Sat, 26 Sep 2020 00:07:52 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c6d9999d1602c8dd10d24038cb7a853fa7675166e2574c22194e21b089f98e`  
		Last Modified: Sat, 26 Sep 2020 00:07:51 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3af868fe329ff3ec48e457c9cb6cf7f6db59ad6d496ad21a9d085ac4c9866e`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97187facc53e9385bbd1faf9f94eec9fd67187acb185b241c342356adec229a`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebb7ad698eeacf880cb61aabb841a2f3fd67885737916aef11b9b6508033594`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b28bc94f5ccc03dc1591e017f819c2b10d6e481b3bee66604e609ae71b449b3`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f091e541c5f573cc9bf8b6d3427495211b798bfb620353216667bd80478ed`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf2458da5062b0b24b86e9f69a30538248926ad9e2b8411d32e5955cb67fe3`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25600a431dfe7d2457a4223132df9f335cc891853d4623583f55f16adfe1760a`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2e4ecbae8bfa668a1e0ff5815f029a57708a6c20c764c77a6a574839eefb82`  
		Last Modified: Sat, 26 Sep 2020 00:07:48 GMT  
		Size: 261.4 KB (261429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f7c356a4c3f5ed1e8c67b8c3832a05e5f651cbbd20f19dda4ee676e779b80f`  
		Last Modified: Sat, 26 Sep 2020 00:07:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:27ffb8b800c563c17e484de51fe024e0e051e9d0095dadda9c5f1db7028ce15b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2.1.1-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:0c81e39f253977e239df5f59cf89da2f5c7f009ce1dab3af9c935b96ace5f111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378453354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b788438493f88710ba4198f5a8e2324ba21a891ac37ad2d9279608278dae239e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:21:26 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:21:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:21:59 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:22:00 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:22:01 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 22:22:01 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 22:22:02 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:22:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:22:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:22:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:22:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:22:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:22:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:22:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:22:07 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:22:08 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:22:09 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:22:23 GMT
RUN caddy version
# Fri, 25 Sep 2020 22:22:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a93d915a3d15febf5cb14d3ce13f84e4e1b59e54251670dffff8c859031c10a`  
		Last Modified: Sat, 26 Sep 2020 00:07:38 GMT  
		Size: 9.2 MB (9161113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af424f647689600c8a89cb1e4745cfc5f8a9ec3fa8403d1284007e4f18227c3c`  
		Last Modified: Sat, 26 Sep 2020 00:07:35 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a325c5e893eb9c1eee88bc23abc49cb3bd3981f0ad75bc13f858ceef122813d`  
		Last Modified: Sat, 26 Sep 2020 00:07:40 GMT  
		Size: 17.7 MB (17693393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03255d53b60da941950d8ba5851576b778efc2e7c2cc8226f619ba710c2c71c`  
		Last Modified: Sat, 26 Sep 2020 00:07:34 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aedc819f3a24e1c512e9bd88ba7fe3534e2825040017f12962240208308ee1`  
		Last Modified: Sat, 26 Sep 2020 00:07:34 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbccf79a85ad8d68e31983400cf9cdb914b809b9fbf8af979bb630bd8fb734f`  
		Last Modified: Sat, 26 Sep 2020 00:07:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0347ef53e57ae098b9720a743c36081805b1c00154ce5516b5e1722b31ce7db3`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4366217d729e94916c5bc4f011e863c4436a4f0e28e4aaa7dd38003881c8bfe4`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801beab1a0fa531e11c5c71fe5f9f56f943dd6fef67da4a8816e89deff12a6ef`  
		Last Modified: Sat, 26 Sep 2020 00:07:32 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b7e1df959ce557740ad55e730b687d45931b310c51b9e7163fa43e289c45f`  
		Last Modified: Sat, 26 Sep 2020 00:07:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765ffe959a7df80c92bc3945ac720d3f343f230085dd6c8f112277977b97fcc`  
		Last Modified: Sat, 26 Sep 2020 00:07:30 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c7299920606443a615204b88ae0b26d76f566ae80edb84a43420e971ab8279`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfff45371f5fa6f168f03bf11bbb1f1d751d56c056a3b839aec270c6b276d74`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758bdbc1a34c4a22c92f52b973388589243178ed62087eede3079f411b8dd061`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb7fb0b899cafbd14fde4f7903c37dd72bdf91a0444cce9da878c29d80027ac`  
		Last Modified: Sat, 26 Sep 2020 00:07:29 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62de917f277d9dd32c53e7132b66397808f4a1db49da287b123f906e3956c2eb`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ceef103e926f07af4c4d9419212cf30c0e8fa54adb173e4eb4713d2a01563e`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe48c00ec807e1297e9bb0011a8223135ae2228a413fd77bc6ed8075d842f6`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac963d0f2ed9ce1bae553fa884a12c187e56d3b5f15ffb00e7a5472c667be73`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 306.2 KB (306189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087f889bde7ffdb3305c8da1fa9e5474b8bf585fb276ad612928d92f3bcb1ff7`  
		Last Modified: Sat, 26 Sep 2020 00:07:26 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:817081568dafc454cdfec870956e8a7cbe8053551e5645b85f85a24eabadd1ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.1.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:3eaa72122a1c8777eebb9cb70237412d32f5d00d61deb258a7297dcc01a3915e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772324795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44bcb3197a91f6005135d9d64c534684de99522992a8b00ab5a4b53084889c1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:23:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/506330b23c5cce43a9352179e7977a684678fbaf/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:23:45 GMT
ENV CADDY_VERSION=v2.1.1
# Fri, 25 Sep 2020 22:25:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:25:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:25:11 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:25:12 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 22:25:13 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 22:25:14 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Fri, 25 Sep 2020 22:25:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:25:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:25:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:25:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:25:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:25:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:25:19 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:25:19 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:25:20 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:26:03 GMT
RUN caddy version
# Fri, 25 Sep 2020 22:26:04 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d72b7607b806beed4aafbaccee5c30d613fa762498a797c526cef45222ec10`  
		Last Modified: Sat, 26 Sep 2020 00:08:01 GMT  
		Size: 9.9 MB (9905052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731e7579ab3965dda5a9e41c556c4ca32ccdae9be5ec6e7f46bd647f1fe63891`  
		Last Modified: Sat, 26 Sep 2020 00:07:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fff091c5777968177457a4e9c3aadc893e97f676d024ff5d237158f6c11da7a`  
		Last Modified: Sat, 26 Sep 2020 00:08:02 GMT  
		Size: 22.9 MB (22883540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d05a19446e8af754abceeb85b4631270875c30039d1c3b18a2be62a87fa8c31`  
		Last Modified: Sat, 26 Sep 2020 00:07:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a81327f32b6df82f48e52941f7c74fc59329d2c2d19cb7e67ad728e1bde546`  
		Last Modified: Sat, 26 Sep 2020 00:07:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507b4bf1c0aeb5d728e5277920623c8cb340b2e022f0c2b1e4f56e48528325c6`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b499a6f00e79ce856374f971408bbef25bacc81b012dbd23d2a029397de8238`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92048406361df5dd644d39ff147bc808ada0abdbc5be7589ce6acc74cb806bb9`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b3fb321d9fd8cc3646329da5b16664e63a57f8103630ff5d0fdb9aa55eb704`  
		Last Modified: Sat, 26 Sep 2020 00:07:53 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8c4aa6d8ea1a517610a94bbc5e569df76d6e4a4b4848094972f3434e750472`  
		Last Modified: Sat, 26 Sep 2020 00:07:52 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c6d9999d1602c8dd10d24038cb7a853fa7675166e2574c22194e21b089f98e`  
		Last Modified: Sat, 26 Sep 2020 00:07:51 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3af868fe329ff3ec48e457c9cb6cf7f6db59ad6d496ad21a9d085ac4c9866e`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97187facc53e9385bbd1faf9f94eec9fd67187acb185b241c342356adec229a`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebb7ad698eeacf880cb61aabb841a2f3fd67885737916aef11b9b6508033594`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b28bc94f5ccc03dc1591e017f819c2b10d6e481b3bee66604e609ae71b449b3`  
		Last Modified: Sat, 26 Sep 2020 00:07:50 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f091e541c5f573cc9bf8b6d3427495211b798bfb620353216667bd80478ed`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf2458da5062b0b24b86e9f69a30538248926ad9e2b8411d32e5955cb67fe3`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25600a431dfe7d2457a4223132df9f335cc891853d4623583f55f16adfe1760a`  
		Last Modified: Sat, 26 Sep 2020 00:07:47 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2e4ecbae8bfa668a1e0ff5815f029a57708a6c20c764c77a6a574839eefb82`  
		Last Modified: Sat, 26 Sep 2020 00:07:48 GMT  
		Size: 261.4 KB (261429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f7c356a4c3f5ed1e8c67b8c3832a05e5f651cbbd20f19dda4ee676e779b80f`  
		Last Modified: Sat, 26 Sep 2020 00:07:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0`

```console
$ docker pull caddy@sha256:878e0f076a0c34ddf9f15af052a4fd802aa5b7e69393582655a4fa3755876db8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.2.0` - linux; amd64

```console
$ docker pull caddy@sha256:7210e033f1b7846a51ad4e7e0412f5eecff286aa706500698fbea1f89c316357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14632306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6f01784bcc9de68ae349a8c782c82c8d54f642f6cbadb2472567ea33e69cf0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:27:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:35 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:36 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:38 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bea3a62f2eb8bdd91cf1d01de5e62aa88dbcd8e5834f5dd686a4f1a482531`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 5.8 KB (5761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c6d72ce944f51161d2c13a01dde2210e77bb69c72cbd54e3125a34d60d899`  
		Last Modified: Fri, 25 Sep 2020 22:28:11 GMT  
		Size: 11.5 MB (11528869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e626bfeb2f84ef9a852704892ac16a98c0562469db9c76430725e5c18a998ddb`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c8ad488eec7c77aa1c7781b7a72a8d945481bdd0cb7ccb70880d9b925873048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f98716bd7a8a9c2ef8aa29c6650238e67c38bdb8293c65fee78840359abf69`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:50:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:50:11 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:50:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:50:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:50:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:50:20 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:50:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:50:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:50:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:50:27 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:50:28 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:50:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf9fef63ad932b076740c7fd4eac18d505c2e815b2b27093fae4a1037c1f83`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4febe5cd2333cc513bb8556e642ebf16c47e8b19d55ca0a5ea133b0ac51ffb6`  
		Last Modified: Fri, 25 Sep 2020 22:51:22 GMT  
		Size: 10.9 MB (10871161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a4a456aa5012b57a14ca79cf84c1fcadb9921dacbceabaa51276b470026164`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f7cf9f964eeea33eafd618e61be6df5924aeb7554b18ebf67553d7b6b4b87c4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13563595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9c246982f6b6958d5da2a3fd34536f8ac51c0bb7d8b9f5dac90402a50362ae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:58:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:58:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:58:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:58:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:58:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:58:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:58:40 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:58:41 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:42 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:51 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f21378d6028fa7cda0d5b592cd8b633c405139cc47eee9863c2b21da4378b`  
		Last Modified: Fri, 25 Sep 2020 22:59:48 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665bdf05fdd3470eab6a6ffbc672a036b9fd454b448b462f016d7ca8ef6948`  
		Last Modified: Fri, 25 Sep 2020 22:59:51 GMT  
		Size: 10.9 MB (10851606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff23fb2f1e176ebd5c38157ac164416de40bede15eda73c657fcd72ab44cbf4`  
		Last Modified: Fri, 25 Sep 2020 22:59:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fd7be1e3e7e8f22025c4c7c932ed959e20a042800583b99d221d49210d2256b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13537918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdda1ab60a0a087288e1096da6b835d6d0492ace07c13f12b7ae57fc0aa31fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:18 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:40:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:40:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:40:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:40:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:40:26 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:40:27 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:40:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:40:33 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:40:34 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:40:35 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:40:35 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:40:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bbc79642b3dde186ddb45804729b84a8d010ca521d5c376311e2f613371675`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737d74b46f3ab6089d70958b2003334d319108e095e574ccb5513b8df65957b`  
		Last Modified: Fri, 25 Sep 2020 22:41:26 GMT  
		Size: 10.5 MB (10523576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bccfced4019a7c0a8f4727d9564f261cc2cea2f152604c090c8e1534648917`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:1f9ba55d19fd2ec980dbaeab620562f227dcf0d7ced312dc989d275783c346eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13288765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3fce9822eca46a2dd633cf719e3ed86a1381b29ecaf6869f8959e53899d0e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:41 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:09 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:38 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:47 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:42:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:42:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:42:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:42:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:42:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:42:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:42:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:42:53 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:42:59 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:43:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6899a5c1a337a29052e5f09180d092a86821dcf3d513b96fdf5db876ec3d6368`  
		Last Modified: Fri, 25 Sep 2020 22:45:34 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5fe5c56024bfb32687701ff11f9c64f76889469f8562abad35c6b11862a8cb`  
		Last Modified: Fri, 25 Sep 2020 22:45:35 GMT  
		Size: 10.2 MB (10175209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09e4037c29b877b9d6dc22577ae3f8283f506d76525794858646d23a4c596`  
		Last Modified: Fri, 25 Sep 2020 22:45:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0` - linux; s390x

```console
$ docker pull caddy@sha256:aab2bff384d7eeaac65e97fe65c9f60f11a3515ae789192681455c483e7849d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14069343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036d0863bbc70fc945f1013ac5fc1b1ffa1f292eafc9e5cb9b6167ae03031199`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:41:44 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:50 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b62d245db5345045e7a29f409c7a0109545e93366793659a9538d863745398`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd84433ce0180dc40fb2dfc528d8186c247a35a24b5868a7b6065989bf0ee684`  
		Last Modified: Fri, 25 Sep 2020 22:42:26 GMT  
		Size: 11.2 MB (11196639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b4a42908e611c3b87202fd7fa709303806890837e261ae5a76d427925c7825`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-alpine`

```console
$ docker pull caddy@sha256:7367adca165f92427bf9f63732334d37213e92b1d8800da194dbd7bfbcb87452
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.0-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:7210e033f1b7846a51ad4e7e0412f5eecff286aa706500698fbea1f89c316357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14632306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6f01784bcc9de68ae349a8c782c82c8d54f642f6cbadb2472567ea33e69cf0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:27:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:35 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:36 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:38 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bea3a62f2eb8bdd91cf1d01de5e62aa88dbcd8e5834f5dd686a4f1a482531`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 5.8 KB (5761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c6d72ce944f51161d2c13a01dde2210e77bb69c72cbd54e3125a34d60d899`  
		Last Modified: Fri, 25 Sep 2020 22:28:11 GMT  
		Size: 11.5 MB (11528869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e626bfeb2f84ef9a852704892ac16a98c0562469db9c76430725e5c18a998ddb`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c8ad488eec7c77aa1c7781b7a72a8d945481bdd0cb7ccb70880d9b925873048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f98716bd7a8a9c2ef8aa29c6650238e67c38bdb8293c65fee78840359abf69`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:50:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:50:11 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:50:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:50:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:50:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:50:20 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:50:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:50:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:50:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:50:27 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:50:28 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:50:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf9fef63ad932b076740c7fd4eac18d505c2e815b2b27093fae4a1037c1f83`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4febe5cd2333cc513bb8556e642ebf16c47e8b19d55ca0a5ea133b0ac51ffb6`  
		Last Modified: Fri, 25 Sep 2020 22:51:22 GMT  
		Size: 10.9 MB (10871161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a4a456aa5012b57a14ca79cf84c1fcadb9921dacbceabaa51276b470026164`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f7cf9f964eeea33eafd618e61be6df5924aeb7554b18ebf67553d7b6b4b87c4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13563595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9c246982f6b6958d5da2a3fd34536f8ac51c0bb7d8b9f5dac90402a50362ae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:58:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:58:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:58:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:58:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:58:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:58:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:58:40 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:58:41 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:42 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:51 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f21378d6028fa7cda0d5b592cd8b633c405139cc47eee9863c2b21da4378b`  
		Last Modified: Fri, 25 Sep 2020 22:59:48 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665bdf05fdd3470eab6a6ffbc672a036b9fd454b448b462f016d7ca8ef6948`  
		Last Modified: Fri, 25 Sep 2020 22:59:51 GMT  
		Size: 10.9 MB (10851606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff23fb2f1e176ebd5c38157ac164416de40bede15eda73c657fcd72ab44cbf4`  
		Last Modified: Fri, 25 Sep 2020 22:59:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fd7be1e3e7e8f22025c4c7c932ed959e20a042800583b99d221d49210d2256b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13537918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdda1ab60a0a087288e1096da6b835d6d0492ace07c13f12b7ae57fc0aa31fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:18 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:40:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:40:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:40:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:40:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:40:26 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:40:27 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:40:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:40:33 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:40:34 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:40:35 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:40:35 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:40:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bbc79642b3dde186ddb45804729b84a8d010ca521d5c376311e2f613371675`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737d74b46f3ab6089d70958b2003334d319108e095e574ccb5513b8df65957b`  
		Last Modified: Fri, 25 Sep 2020 22:41:26 GMT  
		Size: 10.5 MB (10523576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bccfced4019a7c0a8f4727d9564f261cc2cea2f152604c090c8e1534648917`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1f9ba55d19fd2ec980dbaeab620562f227dcf0d7ced312dc989d275783c346eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13288765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3fce9822eca46a2dd633cf719e3ed86a1381b29ecaf6869f8959e53899d0e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:41 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:09 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:38 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:47 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:42:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:42:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:42:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:42:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:42:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:42:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:42:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:42:53 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:42:59 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:43:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6899a5c1a337a29052e5f09180d092a86821dcf3d513b96fdf5db876ec3d6368`  
		Last Modified: Fri, 25 Sep 2020 22:45:34 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5fe5c56024bfb32687701ff11f9c64f76889469f8562abad35c6b11862a8cb`  
		Last Modified: Fri, 25 Sep 2020 22:45:35 GMT  
		Size: 10.2 MB (10175209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09e4037c29b877b9d6dc22577ae3f8283f506d76525794858646d23a4c596`  
		Last Modified: Fri, 25 Sep 2020 22:45:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:aab2bff384d7eeaac65e97fe65c9f60f11a3515ae789192681455c483e7849d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14069343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036d0863bbc70fc945f1013ac5fc1b1ffa1f292eafc9e5cb9b6167ae03031199`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:41:44 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:50 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b62d245db5345045e7a29f409c7a0109545e93366793659a9538d863745398`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd84433ce0180dc40fb2dfc528d8186c247a35a24b5868a7b6065989bf0ee684`  
		Last Modified: Fri, 25 Sep 2020 22:42:26 GMT  
		Size: 11.2 MB (11196639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b4a42908e611c3b87202fd7fa709303806890837e261ae5a76d427925c7825`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-builder`

```console
$ docker pull caddy@sha256:020d90a1de718717471bd55af55a46e94baf8f814d564e1b71cfacecbc8668a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.2.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:a235adfc9e278c997d31d5f8a6689f0b77d14717715aebb2c68416e6638f29fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120085136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d6c14a9d8a82163a267d5e933b49fb65cf12f39bccf5e698b5f091286eeff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:20:06 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:22:16 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:22:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:45 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871e8e8d7a9e6e0e8b5c74575f14475ace81baa17901d798568eb6fc89c6605`  
		Last Modified: Wed, 09 Sep 2020 22:28:59 GMT  
		Size: 107.3 MB (107287077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73272ec9a57b94a2277ac06d457ca5382aa07be5c17cfddc44e9572e058f01e`  
		Last Modified: Wed, 09 Sep 2020 22:28:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc77d7d3d1a8614ee91da79da91cf0aad076637b63568e8f37506c7753ce627c`  
		Last Modified: Fri, 25 Sep 2020 22:28:18 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcd5e7887fabf6c6917a933aed797cfb46d7bb6fa142178c04b3e3a140eac`  
		Last Modified: Fri, 25 Sep 2020 22:28:17 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e941d493aa7d07e91379d0eda531989523ba28a44b78bcc7edeec9f3987c461`  
		Last Modified: Fri, 25 Sep 2020 22:28:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124796f5ff781b2003a45f3f48668358b8d2537e8b369daf9ae1ee834ef9a2e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115230619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9317396873eb25c0b1c29f66e30506b4d29c7fe5d26e0f056fd6f92e08fb490`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:51:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:53:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:53:57 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:53:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:53:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:54:00 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:50:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:50:39 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:50:40 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33289ebfa0798f70595592ba1a31e18c039bf9047bbf13b9daf83c6bdf47fd9a`  
		Last Modified: Wed, 09 Sep 2020 23:01:48 GMT  
		Size: 103.1 MB (103087634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835f9f7cff0ebd0351d7c28d6324d6466e20a35d1988db525477611b9909550`  
		Last Modified: Wed, 09 Sep 2020 23:01:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5a9ed04456aff68ffe1e84bda9b04c2fa1c359fcd7cb23e64fd328a6d4fe6c`  
		Last Modified: Fri, 25 Sep 2020 22:51:32 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab2b6c0790983f6b3cb40e6ec9f74c969959d84522ec1e2158072b36023f76`  
		Last Modified: Fri, 25 Sep 2020 22:51:30 GMT  
		Size: 1.3 MB (1327361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d30d6da1eff098cd750d1da11bbca28f94d441c7d1a7147d5ed002487fc260`  
		Last Modified: Fri, 25 Sep 2020 22:51:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1335a6af3c755dab10b64471e8d7daf18621a0e495221c118d7d170720811523
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114011080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b423990c53dac245b0994a1b38dc939a4e18a439c40920dda6ad57b03569095`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:01:53 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:04:13 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:04:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:04:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:59:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:59:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:59:05 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:59:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:59:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4617330c6e6b78b275a88d667be57a5b0fb668dab185289351c64522b8bbe65a`  
		Last Modified: Wed, 09 Sep 2020 22:12:18 GMT  
		Size: 102.9 MB (102850878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b43ff2f6d56f9dfa6751a3ea1972340b9102c86f45efdc310d66cd69d482`  
		Last Modified: Wed, 09 Sep 2020 22:11:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18e3ae4626b5fa43914df0ea51e4de5da9432c60cc389a99d9d105c1a9747a`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 7.1 MB (7144989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d5a06d3378d76a591e0da327257e3400f1947261892787c2e454432b59670`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd827ef2105f7c9646773438437f43d1ca68b3c8329573a3a3d341aea1f7f`  
		Last Modified: Fri, 25 Sep 2020 22:59:59 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c87fcf0e1e9653c67e9c57334d79b325b409581f3706af2e9314c03aad6435c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115368932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da11d27cbbbc62784148ff047c6358c9b1e5c1cc10af48dcc14118eaa791a429`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:40:20 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:42:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:42:09 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:42:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:42:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:42:11 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:46 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8529a6b9a6be640bc502712219f1fb2745504a3f39ec97daaf85d4c8264af755`  
		Last Modified: Wed, 09 Sep 2020 22:49:05 GMT  
		Size: 102.6 MB (102567178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45590311c82a93cced41b144bb10045cbd6cc2e5021a4cea50b1a72aa405fc1b`  
		Last Modified: Wed, 09 Sep 2020 22:48:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c054b5ce906c9bc36844a82271f2781122ef429003d967ab45644a8e017c7ffd`  
		Last Modified: Fri, 25 Sep 2020 22:41:36 GMT  
		Size: 8.5 MB (8499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540954645718dfd87b7e29d9ae66a4cd55e5d42335e09b449ef1206a33ca77e5`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf80c30c740156a6daa88423d604ba8ffcec0bab561a94cccabd0596307c6df`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:eab9cbd395418d60b4eec5f86d740ba07a8ce0b44f0ab8d34b9c044a387e889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114548826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d9b8a951a941b518cfcbd3eee3a44db638d5037090e565cce0a8bae1cd7935`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:21:49 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:24:14 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:24:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:24:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:24:53 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:43:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:43:49 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:43:54 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:44:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:44:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:44:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:44:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e5c3bda96921f0fcdc52d34b4e8e57c154d9eeef090c6ca17e00ac1ca58d6`  
		Last Modified: Wed, 09 Sep 2020 22:41:21 GMT  
		Size: 101.3 MB (101250060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb6e866365ec04fdd345e22c049091abf460071fa0470866449b5c14cda08e`  
		Last Modified: Wed, 09 Sep 2020 22:39:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a4b970cfa1f0abf17873192eda639c3d1c128a0daef00315ea38bafa52bc6`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 8.9 MB (8920027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850afabe9996299a0579a7ba31452c4234dd1649f683a4eaea3fbfefa19f4e11`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e4f3516892ff23f9f92d8b0e8bf0013a28bf43e6325c6a8c16f02828292d4`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:5dd072d70669dca77f2bd4761c2a63673c6ea8006cbe6414f91f06bc04b62a0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118955240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d060fa1beb58bdf3d0a8b74347fc3fa0b6d1b8a1ba52aaa54b2575cf4f676570`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:41:59 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:43:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:43:25 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:43:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:43:27 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:57 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eabcd3f00523ec5c8f8dca341969baa7b2786a73abc348fb5f39edf7a6410c6`  
		Last Modified: Wed, 09 Sep 2020 22:47:34 GMT  
		Size: 106.4 MB (106364195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edeb811f26567d876bcc25c7d4c1c9ffb755523494a4c1670fb44b04a763aa`  
		Last Modified: Wed, 09 Sep 2020 22:47:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616042cacfc26da785f94395686f009bfa4b74481d41345619cf42a83dd7e2ab`  
		Last Modified: Fri, 25 Sep 2020 22:42:37 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdb170db1022f72a92dec4c5a24feb5e81a5dd76e620f4a718ef1c40b7b74b2`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f695de8822118cdfa07c995225f5f0136be9571af69c8ab1ac414ed6ec46c31`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:e10c6632f5b914355df26d63e70fe4a940545484c4dcba3bc35b1aa1f7b3962f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2526210904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2eecc555fc90a8bf4df7b518e22b68f8b38700b792314af2260652cf6bad9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:15:13 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:18:02 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:18:04 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 23:34:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:34:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 23:34:22 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:34:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:05:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:05:08 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0bd16fc11b1520dc1e2fbf82d7b0b36994d70d79ea3c40569159fac911fac`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43273506ae0874f7b6fccb1069823c718ac2b4c0fec5f3540db5c58a9676ff0`  
		Last Modified: Wed, 09 Sep 2020 22:35:08 GMT  
		Size: 138.6 MB (138604881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aa717191d2172cc8e9011a90fabfa3424d79be63383da791098f7541f7149`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f497ba25ae265e723ac6ecb5f6f0efbc60a0bf4e9338b137cf1f607bebe8e2`  
		Last Modified: Sat, 26 Sep 2020 00:09:41 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8c2a1389213688db428ddb3b02703700a1dddabd96137985bc4db50173fa0`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213148c55e982488e5df9284b64e0e42d4dbd525d1fac72d90bd185486689f36`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293bc46142c34a773203945723fbcb2b5782ae868a738172b4094865d56cc0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85984a32af8e9bd8bc4e6d9f6d050dfa5fb7de082fd4bb249475e59302986f67`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.8 MB (1801006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2cfe24906f5f1d1eae7cd59d4aa31ef21b7d81df4a9d0188f0431da04a2478`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-builder-alpine`

```console
$ docker pull caddy@sha256:99e0b6a2a88121e1dfafc843314cc5f4dcc633e8416e07fcc3024246a71fe6b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.2.0-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:a235adfc9e278c997d31d5f8a6689f0b77d14717715aebb2c68416e6638f29fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120085136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d6c14a9d8a82163a267d5e933b49fb65cf12f39bccf5e698b5f091286eeff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:20:06 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:22:16 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:22:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:45 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871e8e8d7a9e6e0e8b5c74575f14475ace81baa17901d798568eb6fc89c6605`  
		Last Modified: Wed, 09 Sep 2020 22:28:59 GMT  
		Size: 107.3 MB (107287077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73272ec9a57b94a2277ac06d457ca5382aa07be5c17cfddc44e9572e058f01e`  
		Last Modified: Wed, 09 Sep 2020 22:28:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc77d7d3d1a8614ee91da79da91cf0aad076637b63568e8f37506c7753ce627c`  
		Last Modified: Fri, 25 Sep 2020 22:28:18 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcd5e7887fabf6c6917a933aed797cfb46d7bb6fa142178c04b3e3a140eac`  
		Last Modified: Fri, 25 Sep 2020 22:28:17 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e941d493aa7d07e91379d0eda531989523ba28a44b78bcc7edeec9f3987c461`  
		Last Modified: Fri, 25 Sep 2020 22:28:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124796f5ff781b2003a45f3f48668358b8d2537e8b369daf9ae1ee834ef9a2e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115230619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9317396873eb25c0b1c29f66e30506b4d29c7fe5d26e0f056fd6f92e08fb490`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:51:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:53:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:53:57 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:53:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:53:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:54:00 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:50:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:50:39 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:50:40 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33289ebfa0798f70595592ba1a31e18c039bf9047bbf13b9daf83c6bdf47fd9a`  
		Last Modified: Wed, 09 Sep 2020 23:01:48 GMT  
		Size: 103.1 MB (103087634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835f9f7cff0ebd0351d7c28d6324d6466e20a35d1988db525477611b9909550`  
		Last Modified: Wed, 09 Sep 2020 23:01:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5a9ed04456aff68ffe1e84bda9b04c2fa1c359fcd7cb23e64fd328a6d4fe6c`  
		Last Modified: Fri, 25 Sep 2020 22:51:32 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab2b6c0790983f6b3cb40e6ec9f74c969959d84522ec1e2158072b36023f76`  
		Last Modified: Fri, 25 Sep 2020 22:51:30 GMT  
		Size: 1.3 MB (1327361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d30d6da1eff098cd750d1da11bbca28f94d441c7d1a7147d5ed002487fc260`  
		Last Modified: Fri, 25 Sep 2020 22:51:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1335a6af3c755dab10b64471e8d7daf18621a0e495221c118d7d170720811523
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114011080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b423990c53dac245b0994a1b38dc939a4e18a439c40920dda6ad57b03569095`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:01:53 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:04:13 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:04:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:04:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:59:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:59:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:59:05 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:59:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:59:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4617330c6e6b78b275a88d667be57a5b0fb668dab185289351c64522b8bbe65a`  
		Last Modified: Wed, 09 Sep 2020 22:12:18 GMT  
		Size: 102.9 MB (102850878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b43ff2f6d56f9dfa6751a3ea1972340b9102c86f45efdc310d66cd69d482`  
		Last Modified: Wed, 09 Sep 2020 22:11:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18e3ae4626b5fa43914df0ea51e4de5da9432c60cc389a99d9d105c1a9747a`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 7.1 MB (7144989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d5a06d3378d76a591e0da327257e3400f1947261892787c2e454432b59670`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd827ef2105f7c9646773438437f43d1ca68b3c8329573a3a3d341aea1f7f`  
		Last Modified: Fri, 25 Sep 2020 22:59:59 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c87fcf0e1e9653c67e9c57334d79b325b409581f3706af2e9314c03aad6435c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115368932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da11d27cbbbc62784148ff047c6358c9b1e5c1cc10af48dcc14118eaa791a429`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:40:20 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:42:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:42:09 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:42:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:42:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:42:11 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:46 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8529a6b9a6be640bc502712219f1fb2745504a3f39ec97daaf85d4c8264af755`  
		Last Modified: Wed, 09 Sep 2020 22:49:05 GMT  
		Size: 102.6 MB (102567178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45590311c82a93cced41b144bb10045cbd6cc2e5021a4cea50b1a72aa405fc1b`  
		Last Modified: Wed, 09 Sep 2020 22:48:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c054b5ce906c9bc36844a82271f2781122ef429003d967ab45644a8e017c7ffd`  
		Last Modified: Fri, 25 Sep 2020 22:41:36 GMT  
		Size: 8.5 MB (8499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540954645718dfd87b7e29d9ae66a4cd55e5d42335e09b449ef1206a33ca77e5`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf80c30c740156a6daa88423d604ba8ffcec0bab561a94cccabd0596307c6df`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:eab9cbd395418d60b4eec5f86d740ba07a8ce0b44f0ab8d34b9c044a387e889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114548826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d9b8a951a941b518cfcbd3eee3a44db638d5037090e565cce0a8bae1cd7935`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:21:49 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:24:14 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:24:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:24:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:24:53 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:43:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:43:49 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:43:54 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:44:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:44:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:44:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:44:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e5c3bda96921f0fcdc52d34b4e8e57c154d9eeef090c6ca17e00ac1ca58d6`  
		Last Modified: Wed, 09 Sep 2020 22:41:21 GMT  
		Size: 101.3 MB (101250060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb6e866365ec04fdd345e22c049091abf460071fa0470866449b5c14cda08e`  
		Last Modified: Wed, 09 Sep 2020 22:39:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a4b970cfa1f0abf17873192eda639c3d1c128a0daef00315ea38bafa52bc6`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 8.9 MB (8920027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850afabe9996299a0579a7ba31452c4234dd1649f683a4eaea3fbfefa19f4e11`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e4f3516892ff23f9f92d8b0e8bf0013a28bf43e6325c6a8c16f02828292d4`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5dd072d70669dca77f2bd4761c2a63673c6ea8006cbe6414f91f06bc04b62a0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118955240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d060fa1beb58bdf3d0a8b74347fc3fa0b6d1b8a1ba52aaa54b2575cf4f676570`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:41:59 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:43:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:43:25 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:43:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:43:27 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:57 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eabcd3f00523ec5c8f8dca341969baa7b2786a73abc348fb5f39edf7a6410c6`  
		Last Modified: Wed, 09 Sep 2020 22:47:34 GMT  
		Size: 106.4 MB (106364195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edeb811f26567d876bcc25c7d4c1c9ffb755523494a4c1670fb44b04a763aa`  
		Last Modified: Wed, 09 Sep 2020 22:47:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616042cacfc26da785f94395686f009bfa4b74481d41345619cf42a83dd7e2ab`  
		Last Modified: Fri, 25 Sep 2020 22:42:37 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdb170db1022f72a92dec4c5a24feb5e81a5dd76e620f4a718ef1c40b7b74b2`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f695de8822118cdfa07c995225f5f0136be9571af69c8ab1ac414ed6ec46c31`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9264e33b96f378bb38c4de794e0262cfeca7b13c5d21da79189b2f1013872666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2.2.0-builder-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:e10c6632f5b914355df26d63e70fe4a940545484c4dcba3bc35b1aa1f7b3962f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2526210904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2eecc555fc90a8bf4df7b518e22b68f8b38700b792314af2260652cf6bad9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:15:13 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:18:02 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:18:04 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 23:34:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:34:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 23:34:22 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:34:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:05:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:05:08 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0bd16fc11b1520dc1e2fbf82d7b0b36994d70d79ea3c40569159fac911fac`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43273506ae0874f7b6fccb1069823c718ac2b4c0fec5f3540db5c58a9676ff0`  
		Last Modified: Wed, 09 Sep 2020 22:35:08 GMT  
		Size: 138.6 MB (138604881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aa717191d2172cc8e9011a90fabfa3424d79be63383da791098f7541f7149`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f497ba25ae265e723ac6ecb5f6f0efbc60a0bf4e9338b137cf1f607bebe8e2`  
		Last Modified: Sat, 26 Sep 2020 00:09:41 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8c2a1389213688db428ddb3b02703700a1dddabd96137985bc4db50173fa0`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213148c55e982488e5df9284b64e0e42d4dbd525d1fac72d90bd185486689f36`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293bc46142c34a773203945723fbcb2b5782ae868a738172b4094865d56cc0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85984a32af8e9bd8bc4e6d9f6d050dfa5fb7de082fd4bb249475e59302986f67`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.8 MB (1801006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2cfe24906f5f1d1eae7cd59d4aa31ef21b7d81df4a9d0188f0431da04a2478`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b1d92380682f9b0bad962636255fafec59f2a4e696211a1efec7112ad8a448db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.2.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-windowsservercore`

```console
$ docker pull caddy@sha256:d2331a29eeacab6318030631c9e30cdbdf62811874041f8838bfbd0f7e592f8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.2.0-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.2.0-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:7dade2ad7012a220264a666cb88816602136a902b5111fa2082b30911aa5208d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2.2.0-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:1c47d1b0fa1e418714b016f99aa5f3ad66676111c8191cb1a12b9fe6b6b2faab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.2.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:7367adca165f92427bf9f63732334d37213e92b1d8800da194dbd7bfbcb87452
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
$ docker pull caddy@sha256:7210e033f1b7846a51ad4e7e0412f5eecff286aa706500698fbea1f89c316357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14632306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6f01784bcc9de68ae349a8c782c82c8d54f642f6cbadb2472567ea33e69cf0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:27:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:35 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:36 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:38 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bea3a62f2eb8bdd91cf1d01de5e62aa88dbcd8e5834f5dd686a4f1a482531`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 5.8 KB (5761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c6d72ce944f51161d2c13a01dde2210e77bb69c72cbd54e3125a34d60d899`  
		Last Modified: Fri, 25 Sep 2020 22:28:11 GMT  
		Size: 11.5 MB (11528869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e626bfeb2f84ef9a852704892ac16a98c0562469db9c76430725e5c18a998ddb`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c8ad488eec7c77aa1c7781b7a72a8d945481bdd0cb7ccb70880d9b925873048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f98716bd7a8a9c2ef8aa29c6650238e67c38bdb8293c65fee78840359abf69`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:50:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:50:11 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:50:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:50:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:50:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:50:20 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:50:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:50:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:50:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:50:27 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:50:28 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:50:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf9fef63ad932b076740c7fd4eac18d505c2e815b2b27093fae4a1037c1f83`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4febe5cd2333cc513bb8556e642ebf16c47e8b19d55ca0a5ea133b0ac51ffb6`  
		Last Modified: Fri, 25 Sep 2020 22:51:22 GMT  
		Size: 10.9 MB (10871161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a4a456aa5012b57a14ca79cf84c1fcadb9921dacbceabaa51276b470026164`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f7cf9f964eeea33eafd618e61be6df5924aeb7554b18ebf67553d7b6b4b87c4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13563595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9c246982f6b6958d5da2a3fd34536f8ac51c0bb7d8b9f5dac90402a50362ae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:58:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:58:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:58:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:58:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:58:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:58:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:58:40 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:58:41 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:42 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:51 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f21378d6028fa7cda0d5b592cd8b633c405139cc47eee9863c2b21da4378b`  
		Last Modified: Fri, 25 Sep 2020 22:59:48 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665bdf05fdd3470eab6a6ffbc672a036b9fd454b448b462f016d7ca8ef6948`  
		Last Modified: Fri, 25 Sep 2020 22:59:51 GMT  
		Size: 10.9 MB (10851606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff23fb2f1e176ebd5c38157ac164416de40bede15eda73c657fcd72ab44cbf4`  
		Last Modified: Fri, 25 Sep 2020 22:59:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fd7be1e3e7e8f22025c4c7c932ed959e20a042800583b99d221d49210d2256b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13537918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdda1ab60a0a087288e1096da6b835d6d0492ace07c13f12b7ae57fc0aa31fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:18 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:40:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:40:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:40:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:40:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:40:26 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:40:27 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:40:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:40:33 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:40:34 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:40:35 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:40:35 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:40:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bbc79642b3dde186ddb45804729b84a8d010ca521d5c376311e2f613371675`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737d74b46f3ab6089d70958b2003334d319108e095e574ccb5513b8df65957b`  
		Last Modified: Fri, 25 Sep 2020 22:41:26 GMT  
		Size: 10.5 MB (10523576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bccfced4019a7c0a8f4727d9564f261cc2cea2f152604c090c8e1534648917`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1f9ba55d19fd2ec980dbaeab620562f227dcf0d7ced312dc989d275783c346eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13288765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3fce9822eca46a2dd633cf719e3ed86a1381b29ecaf6869f8959e53899d0e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:41 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:09 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:38 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:47 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:42:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:42:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:42:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:42:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:42:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:42:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:42:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:42:53 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:42:59 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:43:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6899a5c1a337a29052e5f09180d092a86821dcf3d513b96fdf5db876ec3d6368`  
		Last Modified: Fri, 25 Sep 2020 22:45:34 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5fe5c56024bfb32687701ff11f9c64f76889469f8562abad35c6b11862a8cb`  
		Last Modified: Fri, 25 Sep 2020 22:45:35 GMT  
		Size: 10.2 MB (10175209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09e4037c29b877b9d6dc22577ae3f8283f506d76525794858646d23a4c596`  
		Last Modified: Fri, 25 Sep 2020 22:45:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:aab2bff384d7eeaac65e97fe65c9f60f11a3515ae789192681455c483e7849d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14069343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036d0863bbc70fc945f1013ac5fc1b1ffa1f292eafc9e5cb9b6167ae03031199`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:41:44 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:50 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b62d245db5345045e7a29f409c7a0109545e93366793659a9538d863745398`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd84433ce0180dc40fb2dfc528d8186c247a35a24b5868a7b6065989bf0ee684`  
		Last Modified: Fri, 25 Sep 2020 22:42:26 GMT  
		Size: 11.2 MB (11196639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b4a42908e611c3b87202fd7fa709303806890837e261ae5a76d427925c7825`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:020d90a1de718717471bd55af55a46e94baf8f814d564e1b71cfacecbc8668a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:a235adfc9e278c997d31d5f8a6689f0b77d14717715aebb2c68416e6638f29fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120085136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d6c14a9d8a82163a267d5e933b49fb65cf12f39bccf5e698b5f091286eeff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:20:06 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:22:16 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:22:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:45 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871e8e8d7a9e6e0e8b5c74575f14475ace81baa17901d798568eb6fc89c6605`  
		Last Modified: Wed, 09 Sep 2020 22:28:59 GMT  
		Size: 107.3 MB (107287077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73272ec9a57b94a2277ac06d457ca5382aa07be5c17cfddc44e9572e058f01e`  
		Last Modified: Wed, 09 Sep 2020 22:28:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc77d7d3d1a8614ee91da79da91cf0aad076637b63568e8f37506c7753ce627c`  
		Last Modified: Fri, 25 Sep 2020 22:28:18 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcd5e7887fabf6c6917a933aed797cfb46d7bb6fa142178c04b3e3a140eac`  
		Last Modified: Fri, 25 Sep 2020 22:28:17 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e941d493aa7d07e91379d0eda531989523ba28a44b78bcc7edeec9f3987c461`  
		Last Modified: Fri, 25 Sep 2020 22:28:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124796f5ff781b2003a45f3f48668358b8d2537e8b369daf9ae1ee834ef9a2e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115230619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9317396873eb25c0b1c29f66e30506b4d29c7fe5d26e0f056fd6f92e08fb490`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:51:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:53:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:53:57 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:53:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:53:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:54:00 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:50:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:50:39 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:50:40 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33289ebfa0798f70595592ba1a31e18c039bf9047bbf13b9daf83c6bdf47fd9a`  
		Last Modified: Wed, 09 Sep 2020 23:01:48 GMT  
		Size: 103.1 MB (103087634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835f9f7cff0ebd0351d7c28d6324d6466e20a35d1988db525477611b9909550`  
		Last Modified: Wed, 09 Sep 2020 23:01:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5a9ed04456aff68ffe1e84bda9b04c2fa1c359fcd7cb23e64fd328a6d4fe6c`  
		Last Modified: Fri, 25 Sep 2020 22:51:32 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab2b6c0790983f6b3cb40e6ec9f74c969959d84522ec1e2158072b36023f76`  
		Last Modified: Fri, 25 Sep 2020 22:51:30 GMT  
		Size: 1.3 MB (1327361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d30d6da1eff098cd750d1da11bbca28f94d441c7d1a7147d5ed002487fc260`  
		Last Modified: Fri, 25 Sep 2020 22:51:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1335a6af3c755dab10b64471e8d7daf18621a0e495221c118d7d170720811523
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114011080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b423990c53dac245b0994a1b38dc939a4e18a439c40920dda6ad57b03569095`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:01:53 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:04:13 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:04:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:04:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:59:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:59:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:59:05 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:59:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:59:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4617330c6e6b78b275a88d667be57a5b0fb668dab185289351c64522b8bbe65a`  
		Last Modified: Wed, 09 Sep 2020 22:12:18 GMT  
		Size: 102.9 MB (102850878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b43ff2f6d56f9dfa6751a3ea1972340b9102c86f45efdc310d66cd69d482`  
		Last Modified: Wed, 09 Sep 2020 22:11:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18e3ae4626b5fa43914df0ea51e4de5da9432c60cc389a99d9d105c1a9747a`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 7.1 MB (7144989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d5a06d3378d76a591e0da327257e3400f1947261892787c2e454432b59670`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd827ef2105f7c9646773438437f43d1ca68b3c8329573a3a3d341aea1f7f`  
		Last Modified: Fri, 25 Sep 2020 22:59:59 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c87fcf0e1e9653c67e9c57334d79b325b409581f3706af2e9314c03aad6435c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115368932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da11d27cbbbc62784148ff047c6358c9b1e5c1cc10af48dcc14118eaa791a429`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:40:20 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:42:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:42:09 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:42:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:42:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:42:11 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:46 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8529a6b9a6be640bc502712219f1fb2745504a3f39ec97daaf85d4c8264af755`  
		Last Modified: Wed, 09 Sep 2020 22:49:05 GMT  
		Size: 102.6 MB (102567178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45590311c82a93cced41b144bb10045cbd6cc2e5021a4cea50b1a72aa405fc1b`  
		Last Modified: Wed, 09 Sep 2020 22:48:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c054b5ce906c9bc36844a82271f2781122ef429003d967ab45644a8e017c7ffd`  
		Last Modified: Fri, 25 Sep 2020 22:41:36 GMT  
		Size: 8.5 MB (8499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540954645718dfd87b7e29d9ae66a4cd55e5d42335e09b449ef1206a33ca77e5`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf80c30c740156a6daa88423d604ba8ffcec0bab561a94cccabd0596307c6df`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:eab9cbd395418d60b4eec5f86d740ba07a8ce0b44f0ab8d34b9c044a387e889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114548826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d9b8a951a941b518cfcbd3eee3a44db638d5037090e565cce0a8bae1cd7935`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:21:49 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:24:14 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:24:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:24:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:24:53 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:43:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:43:49 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:43:54 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:44:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:44:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:44:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:44:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e5c3bda96921f0fcdc52d34b4e8e57c154d9eeef090c6ca17e00ac1ca58d6`  
		Last Modified: Wed, 09 Sep 2020 22:41:21 GMT  
		Size: 101.3 MB (101250060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb6e866365ec04fdd345e22c049091abf460071fa0470866449b5c14cda08e`  
		Last Modified: Wed, 09 Sep 2020 22:39:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a4b970cfa1f0abf17873192eda639c3d1c128a0daef00315ea38bafa52bc6`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 8.9 MB (8920027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850afabe9996299a0579a7ba31452c4234dd1649f683a4eaea3fbfefa19f4e11`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e4f3516892ff23f9f92d8b0e8bf0013a28bf43e6325c6a8c16f02828292d4`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:5dd072d70669dca77f2bd4761c2a63673c6ea8006cbe6414f91f06bc04b62a0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118955240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d060fa1beb58bdf3d0a8b74347fc3fa0b6d1b8a1ba52aaa54b2575cf4f676570`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:41:59 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:43:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:43:25 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:43:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:43:27 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:57 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eabcd3f00523ec5c8f8dca341969baa7b2786a73abc348fb5f39edf7a6410c6`  
		Last Modified: Wed, 09 Sep 2020 22:47:34 GMT  
		Size: 106.4 MB (106364195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edeb811f26567d876bcc25c7d4c1c9ffb755523494a4c1670fb44b04a763aa`  
		Last Modified: Wed, 09 Sep 2020 22:47:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616042cacfc26da785f94395686f009bfa4b74481d41345619cf42a83dd7e2ab`  
		Last Modified: Fri, 25 Sep 2020 22:42:37 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdb170db1022f72a92dec4c5a24feb5e81a5dd76e620f4a718ef1c40b7b74b2`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f695de8822118cdfa07c995225f5f0136be9571af69c8ab1ac414ed6ec46c31`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:e10c6632f5b914355df26d63e70fe4a940545484c4dcba3bc35b1aa1f7b3962f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2526210904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2eecc555fc90a8bf4df7b518e22b68f8b38700b792314af2260652cf6bad9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:15:13 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:18:02 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:18:04 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 23:34:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:34:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 23:34:22 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:34:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:05:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:05:08 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0bd16fc11b1520dc1e2fbf82d7b0b36994d70d79ea3c40569159fac911fac`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43273506ae0874f7b6fccb1069823c718ac2b4c0fec5f3540db5c58a9676ff0`  
		Last Modified: Wed, 09 Sep 2020 22:35:08 GMT  
		Size: 138.6 MB (138604881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aa717191d2172cc8e9011a90fabfa3424d79be63383da791098f7541f7149`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f497ba25ae265e723ac6ecb5f6f0efbc60a0bf4e9338b137cf1f607bebe8e2`  
		Last Modified: Sat, 26 Sep 2020 00:09:41 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8c2a1389213688db428ddb3b02703700a1dddabd96137985bc4db50173fa0`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213148c55e982488e5df9284b64e0e42d4dbd525d1fac72d90bd185486689f36`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293bc46142c34a773203945723fbcb2b5782ae868a738172b4094865d56cc0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85984a32af8e9bd8bc4e6d9f6d050dfa5fb7de082fd4bb249475e59302986f67`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.8 MB (1801006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2cfe24906f5f1d1eae7cd59d4aa31ef21b7d81df4a9d0188f0431da04a2478`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:99e0b6a2a88121e1dfafc843314cc5f4dcc633e8416e07fcc3024246a71fe6b1
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
$ docker pull caddy@sha256:a235adfc9e278c997d31d5f8a6689f0b77d14717715aebb2c68416e6638f29fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120085136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d6c14a9d8a82163a267d5e933b49fb65cf12f39bccf5e698b5f091286eeff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:20:06 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:22:16 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:22:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:45 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871e8e8d7a9e6e0e8b5c74575f14475ace81baa17901d798568eb6fc89c6605`  
		Last Modified: Wed, 09 Sep 2020 22:28:59 GMT  
		Size: 107.3 MB (107287077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73272ec9a57b94a2277ac06d457ca5382aa07be5c17cfddc44e9572e058f01e`  
		Last Modified: Wed, 09 Sep 2020 22:28:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc77d7d3d1a8614ee91da79da91cf0aad076637b63568e8f37506c7753ce627c`  
		Last Modified: Fri, 25 Sep 2020 22:28:18 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcd5e7887fabf6c6917a933aed797cfb46d7bb6fa142178c04b3e3a140eac`  
		Last Modified: Fri, 25 Sep 2020 22:28:17 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e941d493aa7d07e91379d0eda531989523ba28a44b78bcc7edeec9f3987c461`  
		Last Modified: Fri, 25 Sep 2020 22:28:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124796f5ff781b2003a45f3f48668358b8d2537e8b369daf9ae1ee834ef9a2e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115230619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9317396873eb25c0b1c29f66e30506b4d29c7fe5d26e0f056fd6f92e08fb490`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:51:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:53:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:53:57 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:53:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:53:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:54:00 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:50:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:50:39 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:50:40 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33289ebfa0798f70595592ba1a31e18c039bf9047bbf13b9daf83c6bdf47fd9a`  
		Last Modified: Wed, 09 Sep 2020 23:01:48 GMT  
		Size: 103.1 MB (103087634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835f9f7cff0ebd0351d7c28d6324d6466e20a35d1988db525477611b9909550`  
		Last Modified: Wed, 09 Sep 2020 23:01:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5a9ed04456aff68ffe1e84bda9b04c2fa1c359fcd7cb23e64fd328a6d4fe6c`  
		Last Modified: Fri, 25 Sep 2020 22:51:32 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab2b6c0790983f6b3cb40e6ec9f74c969959d84522ec1e2158072b36023f76`  
		Last Modified: Fri, 25 Sep 2020 22:51:30 GMT  
		Size: 1.3 MB (1327361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d30d6da1eff098cd750d1da11bbca28f94d441c7d1a7147d5ed002487fc260`  
		Last Modified: Fri, 25 Sep 2020 22:51:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1335a6af3c755dab10b64471e8d7daf18621a0e495221c118d7d170720811523
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114011080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b423990c53dac245b0994a1b38dc939a4e18a439c40920dda6ad57b03569095`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:01:53 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:04:13 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:04:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:04:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:59:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:59:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:59:05 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:59:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:59:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4617330c6e6b78b275a88d667be57a5b0fb668dab185289351c64522b8bbe65a`  
		Last Modified: Wed, 09 Sep 2020 22:12:18 GMT  
		Size: 102.9 MB (102850878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b43ff2f6d56f9dfa6751a3ea1972340b9102c86f45efdc310d66cd69d482`  
		Last Modified: Wed, 09 Sep 2020 22:11:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18e3ae4626b5fa43914df0ea51e4de5da9432c60cc389a99d9d105c1a9747a`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 7.1 MB (7144989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d5a06d3378d76a591e0da327257e3400f1947261892787c2e454432b59670`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd827ef2105f7c9646773438437f43d1ca68b3c8329573a3a3d341aea1f7f`  
		Last Modified: Fri, 25 Sep 2020 22:59:59 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c87fcf0e1e9653c67e9c57334d79b325b409581f3706af2e9314c03aad6435c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115368932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da11d27cbbbc62784148ff047c6358c9b1e5c1cc10af48dcc14118eaa791a429`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:40:20 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:42:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:42:09 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:42:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:42:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:42:11 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:46 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8529a6b9a6be640bc502712219f1fb2745504a3f39ec97daaf85d4c8264af755`  
		Last Modified: Wed, 09 Sep 2020 22:49:05 GMT  
		Size: 102.6 MB (102567178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45590311c82a93cced41b144bb10045cbd6cc2e5021a4cea50b1a72aa405fc1b`  
		Last Modified: Wed, 09 Sep 2020 22:48:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c054b5ce906c9bc36844a82271f2781122ef429003d967ab45644a8e017c7ffd`  
		Last Modified: Fri, 25 Sep 2020 22:41:36 GMT  
		Size: 8.5 MB (8499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540954645718dfd87b7e29d9ae66a4cd55e5d42335e09b449ef1206a33ca77e5`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf80c30c740156a6daa88423d604ba8ffcec0bab561a94cccabd0596307c6df`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:eab9cbd395418d60b4eec5f86d740ba07a8ce0b44f0ab8d34b9c044a387e889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114548826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d9b8a951a941b518cfcbd3eee3a44db638d5037090e565cce0a8bae1cd7935`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:21:49 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:24:14 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:24:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:24:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:24:53 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:43:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:43:49 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:43:54 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:44:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:44:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:44:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:44:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e5c3bda96921f0fcdc52d34b4e8e57c154d9eeef090c6ca17e00ac1ca58d6`  
		Last Modified: Wed, 09 Sep 2020 22:41:21 GMT  
		Size: 101.3 MB (101250060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb6e866365ec04fdd345e22c049091abf460071fa0470866449b5c14cda08e`  
		Last Modified: Wed, 09 Sep 2020 22:39:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a4b970cfa1f0abf17873192eda639c3d1c128a0daef00315ea38bafa52bc6`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 8.9 MB (8920027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850afabe9996299a0579a7ba31452c4234dd1649f683a4eaea3fbfefa19f4e11`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e4f3516892ff23f9f92d8b0e8bf0013a28bf43e6325c6a8c16f02828292d4`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5dd072d70669dca77f2bd4761c2a63673c6ea8006cbe6414f91f06bc04b62a0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118955240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d060fa1beb58bdf3d0a8b74347fc3fa0b6d1b8a1ba52aaa54b2575cf4f676570`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:41:59 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:43:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:43:25 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:43:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:43:27 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:57 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eabcd3f00523ec5c8f8dca341969baa7b2786a73abc348fb5f39edf7a6410c6`  
		Last Modified: Wed, 09 Sep 2020 22:47:34 GMT  
		Size: 106.4 MB (106364195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edeb811f26567d876bcc25c7d4c1c9ffb755523494a4c1670fb44b04a763aa`  
		Last Modified: Wed, 09 Sep 2020 22:47:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616042cacfc26da785f94395686f009bfa4b74481d41345619cf42a83dd7e2ab`  
		Last Modified: Fri, 25 Sep 2020 22:42:37 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdb170db1022f72a92dec4c5a24feb5e81a5dd76e620f4a718ef1c40b7b74b2`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f695de8822118cdfa07c995225f5f0136be9571af69c8ab1ac414ed6ec46c31`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9264e33b96f378bb38c4de794e0262cfeca7b13c5d21da79189b2f1013872666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:e10c6632f5b914355df26d63e70fe4a940545484c4dcba3bc35b1aa1f7b3962f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2526210904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2eecc555fc90a8bf4df7b518e22b68f8b38700b792314af2260652cf6bad9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:15:13 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:18:02 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:18:04 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 23:34:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:34:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 23:34:22 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:34:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:05:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:05:08 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0bd16fc11b1520dc1e2fbf82d7b0b36994d70d79ea3c40569159fac911fac`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43273506ae0874f7b6fccb1069823c718ac2b4c0fec5f3540db5c58a9676ff0`  
		Last Modified: Wed, 09 Sep 2020 22:35:08 GMT  
		Size: 138.6 MB (138604881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aa717191d2172cc8e9011a90fabfa3424d79be63383da791098f7541f7149`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f497ba25ae265e723ac6ecb5f6f0efbc60a0bf4e9338b137cf1f607bebe8e2`  
		Last Modified: Sat, 26 Sep 2020 00:09:41 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8c2a1389213688db428ddb3b02703700a1dddabd96137985bc4db50173fa0`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213148c55e982488e5df9284b64e0e42d4dbd525d1fac72d90bd185486689f36`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293bc46142c34a773203945723fbcb2b5782ae868a738172b4094865d56cc0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85984a32af8e9bd8bc4e6d9f6d050dfa5fb7de082fd4bb249475e59302986f67`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.8 MB (1801006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2cfe24906f5f1d1eae7cd59d4aa31ef21b7d81df4a9d0188f0431da04a2478`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b1d92380682f9b0bad962636255fafec59f2a4e696211a1efec7112ad8a448db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:d2331a29eeacab6318030631c9e30cdbdf62811874041f8838bfbd0f7e592f8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:7dade2ad7012a220264a666cb88816602136a902b5111fa2082b30911aa5208d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:1c47d1b0fa1e418714b016f99aa5f3ad66676111c8191cb1a12b9fe6b6b2faab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:7367adca165f92427bf9f63732334d37213e92b1d8800da194dbd7bfbcb87452
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
$ docker pull caddy@sha256:7210e033f1b7846a51ad4e7e0412f5eecff286aa706500698fbea1f89c316357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14632306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6f01784bcc9de68ae349a8c782c82c8d54f642f6cbadb2472567ea33e69cf0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:27:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:35 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:36 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:38 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bea3a62f2eb8bdd91cf1d01de5e62aa88dbcd8e5834f5dd686a4f1a482531`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 5.8 KB (5761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c6d72ce944f51161d2c13a01dde2210e77bb69c72cbd54e3125a34d60d899`  
		Last Modified: Fri, 25 Sep 2020 22:28:11 GMT  
		Size: 11.5 MB (11528869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e626bfeb2f84ef9a852704892ac16a98c0562469db9c76430725e5c18a998ddb`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c8ad488eec7c77aa1c7781b7a72a8d945481bdd0cb7ccb70880d9b925873048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f98716bd7a8a9c2ef8aa29c6650238e67c38bdb8293c65fee78840359abf69`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:50:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:50:11 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:50:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:50:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:50:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:50:20 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:50:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:50:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:50:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:50:27 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:50:28 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:50:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf9fef63ad932b076740c7fd4eac18d505c2e815b2b27093fae4a1037c1f83`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4febe5cd2333cc513bb8556e642ebf16c47e8b19d55ca0a5ea133b0ac51ffb6`  
		Last Modified: Fri, 25 Sep 2020 22:51:22 GMT  
		Size: 10.9 MB (10871161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a4a456aa5012b57a14ca79cf84c1fcadb9921dacbceabaa51276b470026164`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f7cf9f964eeea33eafd618e61be6df5924aeb7554b18ebf67553d7b6b4b87c4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13563595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9c246982f6b6958d5da2a3fd34536f8ac51c0bb7d8b9f5dac90402a50362ae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:58:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:58:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:58:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:58:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:58:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:58:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:58:40 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:58:41 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:42 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:51 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f21378d6028fa7cda0d5b592cd8b633c405139cc47eee9863c2b21da4378b`  
		Last Modified: Fri, 25 Sep 2020 22:59:48 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665bdf05fdd3470eab6a6ffbc672a036b9fd454b448b462f016d7ca8ef6948`  
		Last Modified: Fri, 25 Sep 2020 22:59:51 GMT  
		Size: 10.9 MB (10851606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff23fb2f1e176ebd5c38157ac164416de40bede15eda73c657fcd72ab44cbf4`  
		Last Modified: Fri, 25 Sep 2020 22:59:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fd7be1e3e7e8f22025c4c7c932ed959e20a042800583b99d221d49210d2256b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13537918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdda1ab60a0a087288e1096da6b835d6d0492ace07c13f12b7ae57fc0aa31fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:18 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:40:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:40:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:40:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:40:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:40:26 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:40:27 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:40:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:40:33 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:40:34 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:40:35 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:40:35 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:40:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bbc79642b3dde186ddb45804729b84a8d010ca521d5c376311e2f613371675`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737d74b46f3ab6089d70958b2003334d319108e095e574ccb5513b8df65957b`  
		Last Modified: Fri, 25 Sep 2020 22:41:26 GMT  
		Size: 10.5 MB (10523576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bccfced4019a7c0a8f4727d9564f261cc2cea2f152604c090c8e1534648917`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1f9ba55d19fd2ec980dbaeab620562f227dcf0d7ced312dc989d275783c346eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13288765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3fce9822eca46a2dd633cf719e3ed86a1381b29ecaf6869f8959e53899d0e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:41 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:09 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:38 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:47 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:42:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:42:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:42:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:42:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:42:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:42:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:42:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:42:53 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:42:59 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:43:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6899a5c1a337a29052e5f09180d092a86821dcf3d513b96fdf5db876ec3d6368`  
		Last Modified: Fri, 25 Sep 2020 22:45:34 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5fe5c56024bfb32687701ff11f9c64f76889469f8562abad35c6b11862a8cb`  
		Last Modified: Fri, 25 Sep 2020 22:45:35 GMT  
		Size: 10.2 MB (10175209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09e4037c29b877b9d6dc22577ae3f8283f506d76525794858646d23a4c596`  
		Last Modified: Fri, 25 Sep 2020 22:45:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:aab2bff384d7eeaac65e97fe65c9f60f11a3515ae789192681455c483e7849d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14069343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036d0863bbc70fc945f1013ac5fc1b1ffa1f292eafc9e5cb9b6167ae03031199`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:41:44 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:50 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b62d245db5345045e7a29f409c7a0109545e93366793659a9538d863745398`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd84433ce0180dc40fb2dfc528d8186c247a35a24b5868a7b6065989bf0ee684`  
		Last Modified: Fri, 25 Sep 2020 22:42:26 GMT  
		Size: 11.2 MB (11196639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b4a42908e611c3b87202fd7fa709303806890837e261ae5a76d427925c7825`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:020d90a1de718717471bd55af55a46e94baf8f814d564e1b71cfacecbc8668a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:a235adfc9e278c997d31d5f8a6689f0b77d14717715aebb2c68416e6638f29fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120085136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d6c14a9d8a82163a267d5e933b49fb65cf12f39bccf5e698b5f091286eeff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:20:06 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:22:16 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:22:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:45 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871e8e8d7a9e6e0e8b5c74575f14475ace81baa17901d798568eb6fc89c6605`  
		Last Modified: Wed, 09 Sep 2020 22:28:59 GMT  
		Size: 107.3 MB (107287077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73272ec9a57b94a2277ac06d457ca5382aa07be5c17cfddc44e9572e058f01e`  
		Last Modified: Wed, 09 Sep 2020 22:28:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc77d7d3d1a8614ee91da79da91cf0aad076637b63568e8f37506c7753ce627c`  
		Last Modified: Fri, 25 Sep 2020 22:28:18 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcd5e7887fabf6c6917a933aed797cfb46d7bb6fa142178c04b3e3a140eac`  
		Last Modified: Fri, 25 Sep 2020 22:28:17 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e941d493aa7d07e91379d0eda531989523ba28a44b78bcc7edeec9f3987c461`  
		Last Modified: Fri, 25 Sep 2020 22:28:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124796f5ff781b2003a45f3f48668358b8d2537e8b369daf9ae1ee834ef9a2e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115230619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9317396873eb25c0b1c29f66e30506b4d29c7fe5d26e0f056fd6f92e08fb490`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:51:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:53:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:53:57 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:53:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:53:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:54:00 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:50:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:50:39 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:50:40 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33289ebfa0798f70595592ba1a31e18c039bf9047bbf13b9daf83c6bdf47fd9a`  
		Last Modified: Wed, 09 Sep 2020 23:01:48 GMT  
		Size: 103.1 MB (103087634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835f9f7cff0ebd0351d7c28d6324d6466e20a35d1988db525477611b9909550`  
		Last Modified: Wed, 09 Sep 2020 23:01:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5a9ed04456aff68ffe1e84bda9b04c2fa1c359fcd7cb23e64fd328a6d4fe6c`  
		Last Modified: Fri, 25 Sep 2020 22:51:32 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab2b6c0790983f6b3cb40e6ec9f74c969959d84522ec1e2158072b36023f76`  
		Last Modified: Fri, 25 Sep 2020 22:51:30 GMT  
		Size: 1.3 MB (1327361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d30d6da1eff098cd750d1da11bbca28f94d441c7d1a7147d5ed002487fc260`  
		Last Modified: Fri, 25 Sep 2020 22:51:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1335a6af3c755dab10b64471e8d7daf18621a0e495221c118d7d170720811523
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114011080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b423990c53dac245b0994a1b38dc939a4e18a439c40920dda6ad57b03569095`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:01:53 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:04:13 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:04:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:04:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:59:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:59:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:59:05 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:59:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:59:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4617330c6e6b78b275a88d667be57a5b0fb668dab185289351c64522b8bbe65a`  
		Last Modified: Wed, 09 Sep 2020 22:12:18 GMT  
		Size: 102.9 MB (102850878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b43ff2f6d56f9dfa6751a3ea1972340b9102c86f45efdc310d66cd69d482`  
		Last Modified: Wed, 09 Sep 2020 22:11:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18e3ae4626b5fa43914df0ea51e4de5da9432c60cc389a99d9d105c1a9747a`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 7.1 MB (7144989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d5a06d3378d76a591e0da327257e3400f1947261892787c2e454432b59670`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd827ef2105f7c9646773438437f43d1ca68b3c8329573a3a3d341aea1f7f`  
		Last Modified: Fri, 25 Sep 2020 22:59:59 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c87fcf0e1e9653c67e9c57334d79b325b409581f3706af2e9314c03aad6435c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115368932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da11d27cbbbc62784148ff047c6358c9b1e5c1cc10af48dcc14118eaa791a429`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:40:20 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:42:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:42:09 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:42:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:42:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:42:11 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:46 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8529a6b9a6be640bc502712219f1fb2745504a3f39ec97daaf85d4c8264af755`  
		Last Modified: Wed, 09 Sep 2020 22:49:05 GMT  
		Size: 102.6 MB (102567178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45590311c82a93cced41b144bb10045cbd6cc2e5021a4cea50b1a72aa405fc1b`  
		Last Modified: Wed, 09 Sep 2020 22:48:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c054b5ce906c9bc36844a82271f2781122ef429003d967ab45644a8e017c7ffd`  
		Last Modified: Fri, 25 Sep 2020 22:41:36 GMT  
		Size: 8.5 MB (8499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540954645718dfd87b7e29d9ae66a4cd55e5d42335e09b449ef1206a33ca77e5`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf80c30c740156a6daa88423d604ba8ffcec0bab561a94cccabd0596307c6df`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:eab9cbd395418d60b4eec5f86d740ba07a8ce0b44f0ab8d34b9c044a387e889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114548826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d9b8a951a941b518cfcbd3eee3a44db638d5037090e565cce0a8bae1cd7935`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:21:49 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:24:14 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:24:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:24:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:24:53 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:43:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:43:49 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:43:54 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:44:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:44:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:44:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:44:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e5c3bda96921f0fcdc52d34b4e8e57c154d9eeef090c6ca17e00ac1ca58d6`  
		Last Modified: Wed, 09 Sep 2020 22:41:21 GMT  
		Size: 101.3 MB (101250060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb6e866365ec04fdd345e22c049091abf460071fa0470866449b5c14cda08e`  
		Last Modified: Wed, 09 Sep 2020 22:39:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a4b970cfa1f0abf17873192eda639c3d1c128a0daef00315ea38bafa52bc6`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 8.9 MB (8920027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850afabe9996299a0579a7ba31452c4234dd1649f683a4eaea3fbfefa19f4e11`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e4f3516892ff23f9f92d8b0e8bf0013a28bf43e6325c6a8c16f02828292d4`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:5dd072d70669dca77f2bd4761c2a63673c6ea8006cbe6414f91f06bc04b62a0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118955240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d060fa1beb58bdf3d0a8b74347fc3fa0b6d1b8a1ba52aaa54b2575cf4f676570`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:41:59 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:43:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:43:25 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:43:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:43:27 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:57 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eabcd3f00523ec5c8f8dca341969baa7b2786a73abc348fb5f39edf7a6410c6`  
		Last Modified: Wed, 09 Sep 2020 22:47:34 GMT  
		Size: 106.4 MB (106364195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edeb811f26567d876bcc25c7d4c1c9ffb755523494a4c1670fb44b04a763aa`  
		Last Modified: Wed, 09 Sep 2020 22:47:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616042cacfc26da785f94395686f009bfa4b74481d41345619cf42a83dd7e2ab`  
		Last Modified: Fri, 25 Sep 2020 22:42:37 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdb170db1022f72a92dec4c5a24feb5e81a5dd76e620f4a718ef1c40b7b74b2`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f695de8822118cdfa07c995225f5f0136be9571af69c8ab1ac414ed6ec46c31`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:e10c6632f5b914355df26d63e70fe4a940545484c4dcba3bc35b1aa1f7b3962f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2526210904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2eecc555fc90a8bf4df7b518e22b68f8b38700b792314af2260652cf6bad9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:15:13 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:18:02 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:18:04 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 23:34:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:34:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 23:34:22 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:34:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:05:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:05:08 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0bd16fc11b1520dc1e2fbf82d7b0b36994d70d79ea3c40569159fac911fac`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43273506ae0874f7b6fccb1069823c718ac2b4c0fec5f3540db5c58a9676ff0`  
		Last Modified: Wed, 09 Sep 2020 22:35:08 GMT  
		Size: 138.6 MB (138604881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aa717191d2172cc8e9011a90fabfa3424d79be63383da791098f7541f7149`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f497ba25ae265e723ac6ecb5f6f0efbc60a0bf4e9338b137cf1f607bebe8e2`  
		Last Modified: Sat, 26 Sep 2020 00:09:41 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8c2a1389213688db428ddb3b02703700a1dddabd96137985bc4db50173fa0`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213148c55e982488e5df9284b64e0e42d4dbd525d1fac72d90bd185486689f36`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293bc46142c34a773203945723fbcb2b5782ae868a738172b4094865d56cc0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85984a32af8e9bd8bc4e6d9f6d050dfa5fb7de082fd4bb249475e59302986f67`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.8 MB (1801006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2cfe24906f5f1d1eae7cd59d4aa31ef21b7d81df4a9d0188f0431da04a2478`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:99e0b6a2a88121e1dfafc843314cc5f4dcc633e8416e07fcc3024246a71fe6b1
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
$ docker pull caddy@sha256:a235adfc9e278c997d31d5f8a6689f0b77d14717715aebb2c68416e6638f29fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120085136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d6c14a9d8a82163a267d5e933b49fb65cf12f39bccf5e698b5f091286eeff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:20:06 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:22:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:22:16 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:22:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:22:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:27:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:27:45 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:27:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:27:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:27:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871e8e8d7a9e6e0e8b5c74575f14475ace81baa17901d798568eb6fc89c6605`  
		Last Modified: Wed, 09 Sep 2020 22:28:59 GMT  
		Size: 107.3 MB (107287077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73272ec9a57b94a2277ac06d457ca5382aa07be5c17cfddc44e9572e058f01e`  
		Last Modified: Wed, 09 Sep 2020 22:28:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc77d7d3d1a8614ee91da79da91cf0aad076637b63568e8f37506c7753ce627c`  
		Last Modified: Fri, 25 Sep 2020 22:28:18 GMT  
		Size: 8.3 MB (8310024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcd5e7887fabf6c6917a933aed797cfb46d7bb6fa142178c04b3e3a140eac`  
		Last Modified: Fri, 25 Sep 2020 22:28:17 GMT  
		Size: 1.4 MB (1407206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e941d493aa7d07e91379d0eda531989523ba28a44b78bcc7edeec9f3987c461`  
		Last Modified: Fri, 25 Sep 2020 22:28:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124796f5ff781b2003a45f3f48668358b8d2537e8b369daf9ae1ee834ef9a2e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115230619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9317396873eb25c0b1c29f66e30506b4d29c7fe5d26e0f056fd6f92e08fb490`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:51:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:53:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:53:57 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:53:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:53:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:54:00 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:50:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:50:39 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:50:40 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:50:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:50:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:50:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33289ebfa0798f70595592ba1a31e18c039bf9047bbf13b9daf83c6bdf47fd9a`  
		Last Modified: Wed, 09 Sep 2020 23:01:48 GMT  
		Size: 103.1 MB (103087634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835f9f7cff0ebd0351d7c28d6324d6466e20a35d1988db525477611b9909550`  
		Last Modified: Wed, 09 Sep 2020 23:01:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5a9ed04456aff68ffe1e84bda9b04c2fa1c359fcd7cb23e64fd328a6d4fe6c`  
		Last Modified: Fri, 25 Sep 2020 22:51:32 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab2b6c0790983f6b3cb40e6ec9f74c969959d84522ec1e2158072b36023f76`  
		Last Modified: Fri, 25 Sep 2020 22:51:30 GMT  
		Size: 1.3 MB (1327361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d30d6da1eff098cd750d1da11bbca28f94d441c7d1a7147d5ed002487fc260`  
		Last Modified: Fri, 25 Sep 2020 22:51:29 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1335a6af3c755dab10b64471e8d7daf18621a0e495221c118d7d170720811523
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114011080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b423990c53dac245b0994a1b38dc939a4e18a439c40920dda6ad57b03569095`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:01:53 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:04:13 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:04:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:04:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:04:17 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:59:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:59:04 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:59:05 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:59:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:59:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:59:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4617330c6e6b78b275a88d667be57a5b0fb668dab185289351c64522b8bbe65a`  
		Last Modified: Wed, 09 Sep 2020 22:12:18 GMT  
		Size: 102.9 MB (102850878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3139b43ff2f6d56f9dfa6751a3ea1972340b9102c86f45efdc310d66cd69d482`  
		Last Modified: Wed, 09 Sep 2020 22:11:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18e3ae4626b5fa43914df0ea51e4de5da9432c60cc389a99d9d105c1a9747a`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 7.1 MB (7144989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3d5a06d3378d76a591e0da327257e3400f1947261892787c2e454432b59670`  
		Last Modified: Fri, 25 Sep 2020 23:00:00 GMT  
		Size: 1.3 MB (1325844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd827ef2105f7c9646773438437f43d1ca68b3c8329573a3a3d341aea1f7f`  
		Last Modified: Fri, 25 Sep 2020 22:59:59 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c87fcf0e1e9653c67e9c57334d79b325b409581f3706af2e9314c03aad6435c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115368932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da11d27cbbbc62784148ff047c6358c9b1e5c1cc10af48dcc14118eaa791a429`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:40:20 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:42:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:42:09 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:42:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:42:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:42:11 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:40:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:40:46 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:40:46 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:40:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:40:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:40:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8529a6b9a6be640bc502712219f1fb2745504a3f39ec97daaf85d4c8264af755`  
		Last Modified: Wed, 09 Sep 2020 22:49:05 GMT  
		Size: 102.6 MB (102567178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45590311c82a93cced41b144bb10045cbd6cc2e5021a4cea50b1a72aa405fc1b`  
		Last Modified: Wed, 09 Sep 2020 22:48:41 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c054b5ce906c9bc36844a82271f2781122ef429003d967ab45644a8e017c7ffd`  
		Last Modified: Fri, 25 Sep 2020 22:41:36 GMT  
		Size: 8.5 MB (8499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540954645718dfd87b7e29d9ae66a4cd55e5d42335e09b449ef1206a33ca77e5`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 1.3 MB (1310178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf80c30c740156a6daa88423d604ba8ffcec0bab561a94cccabd0596307c6df`  
		Last Modified: Fri, 25 Sep 2020 22:41:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:eab9cbd395418d60b4eec5f86d740ba07a8ce0b44f0ab8d34b9c044a387e889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114548826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d9b8a951a941b518cfcbd3eee3a44db638d5037090e565cce0a8bae1cd7935`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:21:49 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:23:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:24:14 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:24:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:24:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:24:53 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:43:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:43:49 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:43:54 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:44:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:44:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:44:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:44:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e5c3bda96921f0fcdc52d34b4e8e57c154d9eeef090c6ca17e00ac1ca58d6`  
		Last Modified: Wed, 09 Sep 2020 22:41:21 GMT  
		Size: 101.3 MB (101250060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb6e866365ec04fdd345e22c049091abf460071fa0470866449b5c14cda08e`  
		Last Modified: Wed, 09 Sep 2020 22:39:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a4b970cfa1f0abf17873192eda639c3d1c128a0daef00315ea38bafa52bc6`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 8.9 MB (8920027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850afabe9996299a0579a7ba31452c4234dd1649f683a4eaea3fbfefa19f4e11`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 1.3 MB (1287791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623e4f3516892ff23f9f92d8b0e8bf0013a28bf43e6325c6a8c16f02828292d4`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5dd072d70669dca77f2bd4761c2a63673c6ea8006cbe6414f91f06bc04b62a0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118955240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d060fa1beb58bdf3d0a8b74347fc3fa0b6d1b8a1ba52aaa54b2575cf4f676570`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:41:59 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:43:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.2.src.tar.gz'; 	sha256='28bf9d0bcde251011caae230a4a05d917b172ea203f2a62f2c2f9533589d4b4d'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:43:25 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:43:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:43:27 GMT
WORKDIR /go
# Fri, 25 Sep 2020 22:41:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 22:41:57 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 25 Sep 2020 22:41:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3d71e90a4b4f3ebc55d79086d5fb4e36d675fd067435b0a2e37f50361e89ceb58a4b8eae43ea502d1b6d1522c3020f1791ffad9a9fbd374883c6202cf9ed67f7' ;; 		armhf)   binArch='armv6'; checksum='243f58f32bba0b6295267ba78ed18c1b36dfd3c8af4ddbe1f8e1fe096a58cb3326d795b19ce06d87b8641fc17d6e8f1fd2ee372af7dca8c844544768cd05c418' ;; 		armv7)   binArch='armv7'; checksum='51c212b44bf21e3d9feb841cb91c93289f5244d7276a7ce4b1eea73121855345190de77f4a87a3e4e1a93cccf6085133b8552de48687c2164277c0766d3404f0' ;; 		aarch64) binArch='arm64'; checksum='13c3184699c20734a5718cad3e4ee8fed52df1eca21d0d3fa5d34a671990bfd1fae23824c7618c0cba1ceac6262b3225f85cbb37cd9c162935c2c367c623e1ea' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='faf068bb6b6086881504699fb92f77f628e36297eda3651021fea40a06a2fa043453a729000d460e530b2772420071b65fdd3915abfdd4d47dbf820e3590393d' ;; 		s390x)   binArch='s390x'; checksum='79527340291d9e2196079c87daabe6fed5f5e354dc3a4a37e59c684aeed910376b472e4d8969c3ae957f1af35272d46e669fa111fcb47bb90a0822aa039970ea' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 25 Sep 2020 22:41:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 25 Sep 2020 22:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eabcd3f00523ec5c8f8dca341969baa7b2786a73abc348fb5f39edf7a6410c6`  
		Last Modified: Wed, 09 Sep 2020 22:47:34 GMT  
		Size: 106.4 MB (106364195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edeb811f26567d876bcc25c7d4c1c9ffb755523494a4c1670fb44b04a763aa`  
		Last Modified: Wed, 09 Sep 2020 22:47:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616042cacfc26da785f94395686f009bfa4b74481d41345619cf42a83dd7e2ab`  
		Last Modified: Fri, 25 Sep 2020 22:42:37 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdb170db1022f72a92dec4c5a24feb5e81a5dd76e620f4a718ef1c40b7b74b2`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 1.4 MB (1388751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f695de8822118cdfa07c995225f5f0136be9571af69c8ab1ac414ed6ec46c31`  
		Last Modified: Fri, 25 Sep 2020 22:42:32 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9264e33b96f378bb38c4de794e0262cfeca7b13c5d21da79189b2f1013872666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:e10c6632f5b914355df26d63e70fe4a940545484c4dcba3bc35b1aa1f7b3962f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2526210904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2eecc555fc90a8bf4df7b518e22b68f8b38700b792314af2260652cf6bad9f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:13:47 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:13:50 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:13:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:15:08 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:15:29 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:15:13 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:18:02 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:18:04 GMT
WORKDIR C:\gopath
# Fri, 25 Sep 2020 23:34:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:34:22 GMT
ENV XCADDY_VERSION=v0.1.5
# Fri, 25 Sep 2020 23:34:22 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:34:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:05:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:05:08 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757096aa14f09e5f9da645853e2c10c872114e53475c0757b392ce50e67cb713`  
		Last Modified: Wed, 09 Sep 2020 13:08:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f648f4c3d1c760e7623e71f68cf991ed10a9679de63fa840eb4b46927333f41`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350e52b1d9d0fe8c4dbbd891839ca89d65de65d2ba76c7c5c0881fe3f7a1ca79`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699f456b528644779ca8c2354f12b2677345e139f373ef6f25270dd992cad503`  
		Last Modified: Wed, 09 Sep 2020 13:08:35 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9558aa7bb8c5a4ba84ad455c9358b2085a78e5d34b827031046440ae2275c9`  
		Last Modified: Wed, 09 Sep 2020 13:09:21 GMT  
		Size: 34.2 MB (34219236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910508ea18aa147253f9f021145a13bebb9669ba98b1bfa595054660c401c11`  
		Last Modified: Wed, 09 Sep 2020 13:08:32 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667bf7a33efb7dd63b41dbdbc3cb3eb63cae5599d607e48a7b6e1fc26c052c0`  
		Last Modified: Wed, 09 Sep 2020 13:08:33 GMT  
		Size: 298.6 KB (298593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0bd16fc11b1520dc1e2fbf82d7b0b36994d70d79ea3c40569159fac911fac`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43273506ae0874f7b6fccb1069823c718ac2b4c0fec5f3540db5c58a9676ff0`  
		Last Modified: Wed, 09 Sep 2020 22:35:08 GMT  
		Size: 138.6 MB (138604881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83aa717191d2172cc8e9011a90fabfa3424d79be63383da791098f7541f7149`  
		Last Modified: Wed, 09 Sep 2020 22:34:40 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f497ba25ae265e723ac6ecb5f6f0efbc60a0bf4e9338b137cf1f607bebe8e2`  
		Last Modified: Sat, 26 Sep 2020 00:09:41 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8c2a1389213688db428ddb3b02703700a1dddabd96137985bc4db50173fa0`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213148c55e982488e5df9284b64e0e42d4dbd525d1fac72d90bd185486689f36`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e293bc46142c34a773203945723fbcb2b5782ae868a738172b4094865d56cc0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85984a32af8e9bd8bc4e6d9f6d050dfa5fb7de082fd4bb249475e59302986f67`  
		Last Modified: Sat, 26 Sep 2020 00:09:39 GMT  
		Size: 1.8 MB (1801006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2cfe24906f5f1d1eae7cd59d4aa31ef21b7d81df4a9d0188f0431da04a2478`  
		Last Modified: Sat, 26 Sep 2020 00:09:38 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b1d92380682f9b0bad962636255fafec59f2a4e696211a1efec7112ad8a448db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:4d936298022722f22223a4642fc9f8ed2434206903a2aee5a0ccfe5e9ef05544
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934739557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6248ead75e6db1387fa77dbcd85cedd9b2dc950a9d18b213b3326fefde8238c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 12:18:29 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Sep 2020 12:18:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Sep 2020 12:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Sep 2020 12:20:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 12:20:38 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Sep 2020 12:21:48 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 22:18:10 GMT
ENV GOLANG_VERSION=1.15.2
# Wed, 09 Sep 2020 22:21:52 GMT
RUN $url = 'https://storage.googleapis.com/golang/go1.15.2.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'e72782cc6de233188c75b06849368826eaa1b8bd9e1cd766db9466a12b7138ca'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 22:21:54 GMT
WORKDIR C:\gopath
# Sat, 26 Sep 2020 00:05:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Sep 2020 00:05:14 GMT
ENV XCADDY_VERSION=v0.1.5
# Sat, 26 Sep 2020 00:05:15 GMT
ENV CADDY_VERSION=v2.2.0
# Sat, 26 Sep 2020 00:05:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 26 Sep 2020 00:06:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.5/xcaddy_0.1.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('9372295e75cb10cff85c609a195b9ac12cea3e9fc3490234d4271d415cd210cfa78116b03d82f008b9519e4d1f6e03fc59c27db80e098798a3065e4e89edd653')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Sat, 26 Sep 2020 00:06:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a145dccd9cb9deebdfe653fe19b1496582b04458867227d362b6b613d922e`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be94e4550a648c900bbe7ab6e436eea72435322878acd5570e9a52fa9e70898`  
		Last Modified: Wed, 09 Sep 2020 13:10:14 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a52cbbc770ffb3c7875b87da8ed562aac385128edad3d5c39ace4e5d595e9`  
		Last Modified: Wed, 09 Sep 2020 13:10:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c649e4c51a75c9b1e836ece5a3fe3998b320bf72c069deaf8cc56819320009`  
		Last Modified: Wed, 09 Sep 2020 13:10:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160f5c38137dc77c8828751c270de2dc0c8fb3fbd4deab6b7501fe96710c396`  
		Last Modified: Wed, 09 Sep 2020 13:10:17 GMT  
		Size: 35.0 MB (34981489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030944457941aa373b68284fbff68917eb429d36dde9315ee45cf2df63c2b1ef`  
		Last Modified: Wed, 09 Sep 2020 13:10:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450314de6715d93af4868f48823694412deeae6a3f5ab0ffd451b6d9819c35ce`  
		Last Modified: Wed, 09 Sep 2020 13:10:05 GMT  
		Size: 5.3 MB (5344951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecedcf46f854e43674c1f8b04765c9c0c03ff1161c19f6e09373cca8fb1870`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236a90691a3efe5b3af8858ded58e25eee17af515c7956a7657a4dee4a607f6`  
		Last Modified: Wed, 09 Sep 2020 22:35:58 GMT  
		Size: 143.8 MB (143819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c35ca8cd2bd30ffb1fac4cc86d9dd60b9a05a4e87f031b71991ac0b252a493`  
		Last Modified: Wed, 09 Sep 2020 22:35:30 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704719653570a43b247a3030f11cf63c17eea86f14550c93e11086cd92bccd91`  
		Last Modified: Sat, 26 Sep 2020 00:10:01 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4be02cdc1d58f084544f98b4558bde317a7d9e19aa05bf7a81a17984c435357`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffc9ead6cbcf1c0c1254c1857fe72f9e36f1e58ef889d99d87c61fd40b1ea3`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158bd0f3dda7216d0c11f44f2b754daae1ff2fbace5ab2bbe9b1a0a489266e6`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19f3bc43a4e492b4c7f0e0b3922dcd08b3df406103c30691115c7e106d9447`  
		Last Modified: Sat, 26 Sep 2020 00:10:03 GMT  
		Size: 11.3 MB (11324045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd4d90d81dcf971d256c25f1278904765a098a866b2878bbecbdd18b3f380`  
		Last Modified: Sat, 26 Sep 2020 00:09:59 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:878e0f076a0c34ddf9f15af052a4fd802aa5b7e69393582655a4fa3755876db8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:7210e033f1b7846a51ad4e7e0412f5eecff286aa706500698fbea1f89c316357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14632306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6f01784bcc9de68ae349a8c782c82c8d54f642f6cbadb2472567ea33e69cf0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:27:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:27:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:27:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:27:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:27:35 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:27:36 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:27:36 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:27:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:27:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:27:38 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:27:38 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:27:39 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5bea3a62f2eb8bdd91cf1d01de5e62aa88dbcd8e5834f5dd686a4f1a482531`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 5.8 KB (5761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c6d72ce944f51161d2c13a01dde2210e77bb69c72cbd54e3125a34d60d899`  
		Last Modified: Fri, 25 Sep 2020 22:28:11 GMT  
		Size: 11.5 MB (11528869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e626bfeb2f84ef9a852704892ac16a98c0562469db9c76430725e5c18a998ddb`  
		Last Modified: Fri, 25 Sep 2020 22:28:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9c8ad488eec7c77aa1c7781b7a72a8d945481bdd0cb7ccb70880d9b925873048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f98716bd7a8a9c2ef8aa29c6650238e67c38bdb8293c65fee78840359abf69`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:50:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:50:11 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:50:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:50:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:50:17 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:50:18 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:50:19 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:50:20 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:50:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:50:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:50:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:50:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:50:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:50:26 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:50:27 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:50:28 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:50:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdf9fef63ad932b076740c7fd4eac18d505c2e815b2b27093fae4a1037c1f83`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4febe5cd2333cc513bb8556e642ebf16c47e8b19d55ca0a5ea133b0ac51ffb6`  
		Last Modified: Fri, 25 Sep 2020 22:51:22 GMT  
		Size: 10.9 MB (10871161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a4a456aa5012b57a14ca79cf84c1fcadb9921dacbceabaa51276b470026164`  
		Last Modified: Fri, 25 Sep 2020 22:51:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f7cf9f964eeea33eafd618e61be6df5924aeb7554b18ebf67553d7b6b4b87c4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13563595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9c246982f6b6958d5da2a3fd34536f8ac51c0bb7d8b9f5dac90402a50362ae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:58:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:58:32 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:58:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:58:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:58:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:58:40 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:58:40 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:58:41 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:58:42 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:58:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:58:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:58:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:58:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:58:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:58:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:58:51 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:58:51 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:58:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f21378d6028fa7cda0d5b592cd8b633c405139cc47eee9863c2b21da4378b`  
		Last Modified: Fri, 25 Sep 2020 22:59:48 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665bdf05fdd3470eab6a6ffbc672a036b9fd454b448b462f016d7ca8ef6948`  
		Last Modified: Fri, 25 Sep 2020 22:59:51 GMT  
		Size: 10.9 MB (10851606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff23fb2f1e176ebd5c38157ac164416de40bede15eda73c657fcd72ab44cbf4`  
		Last Modified: Fri, 25 Sep 2020 22:59:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fd7be1e3e7e8f22025c4c7c932ed959e20a042800583b99d221d49210d2256b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13537918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdda1ab60a0a087288e1096da6b835d6d0492ace07c13f12b7ae57fc0aa31fe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:18 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:40:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:40:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:40:25 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:40:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:40:26 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:40:27 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:40:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:40:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:40:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:40:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:40:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:40:33 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:40:34 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:40:35 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:40:35 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:40:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bbc79642b3dde186ddb45804729b84a8d010ca521d5c376311e2f613371675`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2737d74b46f3ab6089d70958b2003334d319108e095e574ccb5513b8df65957b`  
		Last Modified: Fri, 25 Sep 2020 22:41:26 GMT  
		Size: 10.5 MB (10523576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bccfced4019a7c0a8f4727d9564f261cc2cea2f152604c090c8e1534648917`  
		Last Modified: Fri, 25 Sep 2020 22:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:1f9ba55d19fd2ec980dbaeab620562f227dcf0d7ced312dc989d275783c346eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13288765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3fce9822eca46a2dd633cf719e3ed86a1381b29ecaf6869f8959e53899d0e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:40:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:40:41 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:40:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:09 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:25 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:38 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:47 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:42:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:42:11 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:42:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:42:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:42:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:42:38 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:42:48 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:42:53 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:42:59 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:43:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6899a5c1a337a29052e5f09180d092a86821dcf3d513b96fdf5db876ec3d6368`  
		Last Modified: Fri, 25 Sep 2020 22:45:34 GMT  
		Size: 5.8 KB (5835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5fe5c56024bfb32687701ff11f9c64f76889469f8562abad35c6b11862a8cb`  
		Last Modified: Fri, 25 Sep 2020 22:45:35 GMT  
		Size: 10.2 MB (10175209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb09e4037c29b877b9d6dc22577ae3f8283f506d76525794858646d23a4c596`  
		Last Modified: Fri, 25 Sep 2020 22:45:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:aab2bff384d7eeaac65e97fe65c9f60f11a3515ae789192681455c483e7849d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14069343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036d0863bbc70fc945f1013ac5fc1b1ffa1f292eafc9e5cb9b6167ae03031199`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 25 Sep 2020 22:41:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 25 Sep 2020 22:41:44 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8fb18c1ade5df35c1b2c709ccad45b4893d7c713303446bf05fae22508e69a3c0c0cd354f6c8995262d8e65e08cdf64b5d43a13361ecf1514197081a21b83641' ;; 		armhf)   binArch='armv6'; checksum='79b9162b689ca8e24c6cefad8894262f040d972bef1a3712f94b10f1e405ced58c8b1f6706d8338cf2d8f152cc62f773f12a61614aa88a48d9a4fbea0f40fd3c' ;; 		armv7)   binArch='armv7'; checksum='ec01f438ab2f7e4afaa32da2685cdeeed8cc84d9e03518e713a841101569dad58ae5b66209f871b5adf959d63d19722ba7fcefbe4f583a2d6651feb6dbc65d5c' ;; 		aarch64) binArch='arm64'; checksum='64d63caed8909fa5b13c4e9c50ed2a9a6fe1e2da30b960c08ce995081475d0d7d53bdf5b6c67209f900bdcc49ce5680c61fcf68b2c1e89331a7c68f035659f58' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f4f80cac0df5ecad18f9ee88139c83e6a0eef4518c7dbe3dcf4152fad20be368ed7fd31d5d1930b31cd5f99405c6d67977738ae03dcb33c8f723d9663f876d42' ;; 		s390x)   binArch='s390x'; checksum='04713e3b99e659652504767fdc7908cf38567cdfa7a3fa8557be57c6d438dfefe1cd28d778f7bba95f8c1db5d45f78dc32effd14d03a2a09dd2c5f464e757c82' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 25 Sep 2020 22:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 25 Sep 2020 22:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 25 Sep 2020 22:41:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/config]
# Fri, 25 Sep 2020 22:41:48 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 22:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 22:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 22:41:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 80
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 443
# Fri, 25 Sep 2020 22:41:50 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 22:41:50 GMT
WORKDIR /srv
# Fri, 25 Sep 2020 22:41:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b62d245db5345045e7a29f409c7a0109545e93366793659a9538d863745398`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd84433ce0180dc40fb2dfc528d8186c247a35a24b5868a7b6065989bf0ee684`  
		Last Modified: Fri, 25 Sep 2020 22:42:26 GMT  
		Size: 11.2 MB (11196639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b4a42908e611c3b87202fd7fa709303806890837e261ae5a76d427925c7825`  
		Last Modified: Fri, 25 Sep 2020 22:42:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:d2331a29eeacab6318030631c9e30cdbdf62811874041f8838bfbd0f7e592f8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:7dade2ad7012a220264a666cb88816602136a902b5111fa2082b30911aa5208d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:663a10a3367d11e50538ede9f5d66aa617b65842d054119b4caf4b4caee0f548
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2377072848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348e50d25db6a0855f0c323cf651972ad8bd01cc590d5a96e7e65876efdea4de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 22:59:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 22:59:23 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 22:59:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 22:59:57 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 22:59:58 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 22:59:59 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:00:00 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:00:01 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:00:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:00:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:00:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:00:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:00:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:00:06 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:00:07 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:00:08 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:30:33 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:30:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5289800be51d969b8bedd6fce6f92c21f2f11c6a9b60e9d405bd87a83a55b5c6`  
		Last Modified: Sat, 26 Sep 2020 00:08:48 GMT  
		Size: 9.2 MB (9160763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1375b2569d01761b11f5a89cca0c256ad3e716650302bd0aeb924db40397bf4b`  
		Last Modified: Sat, 26 Sep 2020 00:08:45 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5366f71821cd332305a4bc95d68f230c7c7eb6769ed6366296c6e30e088d649`  
		Last Modified: Sat, 26 Sep 2020 00:08:50 GMT  
		Size: 16.3 MB (16312693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e34e8bb83230b44b8ae661f8c377884d450ec458330cdff74abc08e3d00fab`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5401b2c14040c36c56f57b0e2be63286196d887fd8088620b1d451f47b40bfc6`  
		Last Modified: Sat, 26 Sep 2020 00:08:44 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c3a89a0c95a5fee9bf978e473cac4d4649cc99bc59603f88a958bef521b84`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a057c0b7f15c03ad4a7d1bf82a8ba940f75274c8197cc489e2c54bb46c974`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6aa111d950cbc309f4da038a68062998379c2d88dc99652e01248e226f95b4`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ec7df0440d5e66f22c508751e13a48ec916e0b0612acf346d1207abd9d605`  
		Last Modified: Sat, 26 Sep 2020 00:08:42 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f9eed1ac7d62346f1c5322228d4aea837b0488c2c500f0eda092e58d288f6b`  
		Last Modified: Sat, 26 Sep 2020 00:08:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4f4e18237bf534d16ddf2dca745362f60b0c04de651389e5507b375eb397fa`  
		Last Modified: Sat, 26 Sep 2020 00:08:40 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c77b0e7131df783ccf4713591ec0029144149b973caf3615f1a7c03736505b`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2374656465c6d158b594f83850a1031a1e445ac1f20b95a70bc02eaee3d544`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230246e3e96ec45a0812127a02b438260b059f1897512a055e943b926657c14f`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c653194dd96400291c36fd78bdaa045f17789e1d3468c3414358efc2f7385e`  
		Last Modified: Sat, 26 Sep 2020 00:08:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b543655dd704dabeb9d51f0a6a9fad8754537fe0987e6227296d03f92d11290`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7451d185ce155164e309f36d204848b0590630b94a78b026378e4f3653915d5`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d55a8c762b1ebea35dc64362cab453fdbcdef3cfe7b8e6e2ce8e442fd41ce`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fb2aff838da851801b9942ac9ab3d016f1a3eeac7976d829c771fe3d7014f3`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 306.7 KB (306683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239494c3419efa86f5eec65f328e8a3ab4c84ac641520e48d26f31eaf70d66f`  
		Last Modified: Sat, 26 Sep 2020 00:08:36 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:1c47d1b0fa1e418714b016f99aa5f3ad66676111c8191cb1a12b9fe6b6b2faab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:71e92fc3991e355b12c591fc70cb20b2af7a97e702a407917bf4b91c7a844e0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5770947256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc91db9cb49612683882a30650356b58dc71a5a17d8a45e45966199c52d2d59a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 25 Sep 2020 23:31:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Fri, 25 Sep 2020 23:31:55 GMT
ENV CADDY_VERSION=v2.2.0
# Fri, 25 Sep 2020 23:33:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.2.0/caddy_2.2.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('6f82df7cfcc26087c0794be4a90f4ae5e201820538b61579de48a86bbae23f189eae2a790dfd7de8dcb46ce202a99ed98380871e74aaf9a9e5902918fe5f2273')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Fri, 25 Sep 2020 23:33:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Fri, 25 Sep 2020 23:33:22 GMT
ENV XDG_DATA_HOME=c:/data
# Fri, 25 Sep 2020 23:33:23 GMT
VOLUME [c:/config]
# Fri, 25 Sep 2020 23:33:24 GMT
VOLUME [c:/data]
# Fri, 25 Sep 2020 23:33:25 GMT
LABEL org.opencontainers.image.version=v2.2.0
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 25 Sep 2020 23:33:26 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 25 Sep 2020 23:33:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 25 Sep 2020 23:33:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 25 Sep 2020 23:33:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 25 Sep 2020 23:33:30 GMT
EXPOSE 80
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 443
# Fri, 25 Sep 2020 23:33:31 GMT
EXPOSE 2019
# Fri, 25 Sep 2020 23:34:13 GMT
RUN caddy version
# Fri, 25 Sep 2020 23:34:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39585697033f34555fd08cda2388481a5841fe77ea82c41770ed9d35c641d583`  
		Last Modified: Sat, 26 Sep 2020 00:09:19 GMT  
		Size: 9.9 MB (9906028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ea0364d8679aaaeae9aab83e3da6439e659794f958bb24e89063be83b2a0c`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5655f5e2aea0e80a660bd9f9a251415298c6559aa0beb7a5537ba93023c3c71`  
		Last Modified: Sat, 26 Sep 2020 00:09:21 GMT  
		Size: 21.5 MB (21504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf9bf3a0780671fdda35063a0380e383838b67ce2edb522ddc9bccf852ae0f`  
		Last Modified: Sat, 26 Sep 2020 00:09:15 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b3b297586177b5aa8718d0195d6e714501d2a0a9aaa812e2fc3b97d3c4328`  
		Last Modified: Sat, 26 Sep 2020 00:09:14 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2362c4c405818d45a5c04b12fcbc9b746d1cf464640c12f3525371040759a08`  
		Last Modified: Sat, 26 Sep 2020 00:09:13 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a557640cc4c8fd0927c39c7f7d62fe98bc112f3f80b5f854a8394951b9edf3`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a775d96204df6b918ade760c0141f03bb2d00a8304723669712a22ea7b369`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7f12981c87f669b195288b1c21ce4c3973286e20139220a4157dfcc4be0a`  
		Last Modified: Sat, 26 Sep 2020 00:09:12 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc94fb1ed7ee5e14c38013b19390a8eba8daeac93a1199ad499eb424f66a112c`  
		Last Modified: Sat, 26 Sep 2020 00:09:11 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5679ca7f2641217754e7222857c7b8bf1b66ccae610268146c7650603d8649`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e9af351fd23b793eac6cb044e3aa2308ec824880bbccd0261975be2e03cee5`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b08ec3e064d8da49b4347eb4ff1b22d22e320dba37af89b3019dfc021e88a2`  
		Last Modified: Sat, 26 Sep 2020 00:09:10 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a61c21e514a193da22e2bab69800bafaa5bb05d5ab250ecd6874167bc3af3`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e72d0ef2e0ce55f205a525c4c27409b787ec997233d7b61a3ce22aed086ba41`  
		Last Modified: Sat, 26 Sep 2020 00:09:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df963e827a62a00ce95c0e2eb3601f473c4c163e0f0c722ff1b83536a91705cb`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550122c47edb1124e22cd682951038d1882f42528388f8d6f137574ecf75c60a`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250fe977a22f4c791374a4ae8df162f25f3341a4774b9354ec9a8af1f98fcff3`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a991e61d295e6ce6de2f097984eddae1d5891c6098f9c5fc8f87c07e72c465`  
		Last Modified: Sat, 26 Sep 2020 00:09:07 GMT  
		Size: 261.9 KB (261910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10503427b1af49565aea8c346ae07c6168b6fee80735675adebb41cde94137ca`  
		Last Modified: Sat, 26 Sep 2020 00:09:06 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
