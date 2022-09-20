## `caddy:latest`

```console
$ docker pull caddy@sha256:918c1a90862f95b1f8ea1b5cc869b0d2653bf0d6e18b0010771e17b96155403a
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
$ docker pull caddy@sha256:2c3f65296e448cd18c24f5519b9aec90d63597643cca1330d5f39ff178915b3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17606282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8f90d69a99d8b651c950b602e25aab73c6c2f0fe8d2d753942d2b0903ed823`
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
# Tue, 20 Sep 2022 21:19:16 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 21:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='c05515dd332aa2ef1d50ff7285118deb31aabed336efb8234aaaafe531d0a4525488deffdccd50a20bb9688d4df15464a7d3642956975942528b1705f7811b08' ;; 		armhf)   binArch='armv6'; checksum='e40d557c5c36ae5fe956e1906c3e967f925daf115347188c19b47b118dc7d2c967e8caa8e8a7604a5474114d33552611c85b9135b0ea2c08045635dc6c2a0316' ;; 		armv7)   binArch='armv7'; checksum='6ce633b30541767f93fb1115ab34448d6275856e3dc9fcc31a7ea0472f322838057d23274116181bb15558caac41ddeab89f156880143769485f0b6870afecdb' ;; 		aarch64) binArch='arm64'; checksum='6c7aed21dceec7532ec39c4fa79ba7df6e15cfb9c8802244893de8c6b1998eef79a54810bed271e962c5546be482d6dcc20cbeb9773d23920abbf75694afcbe1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='abd734031a318d69296e0e8776b62267466cbdbc994079db4d9615d15ce79a2369a58317a6d812fe0979bcfe447b15dc5a53f1bad97e9e9b2b4af69a331da17d' ;; 		s390x)   binArch='s390x'; checksum='b727ba39563709f5f53f026e96e6361d0649b9bb7a151f5ecb46b4c1652664516999c708d65b96366b87730ced97b826256fad2ac04db171be893dde815388be' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 20 Sep 2022 21:19:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Sep 2022 21:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 20 Sep 2022 21:19:19 GMT
ENV XDG_DATA_HOME=/data
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 21:19:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 21:19:20 GMT
EXPOSE 80
# Tue, 20 Sep 2022 21:19:21 GMT
EXPOSE 443
# Tue, 20 Sep 2022 21:19:21 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 21:19:21 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 21:19:21 GMT
WORKDIR /srv
# Tue, 20 Sep 2022 21:19:21 GMT
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
	-	`sha256:cc800527c197d6387714ed09dd64d071dde84ac3e1ee779787f6f5ebcc79067f`  
		Last Modified: Tue, 20 Sep 2022 21:19:44 GMT  
		Size: 14.5 MB (14489734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b914d85a1ddddf9d3311ddf344777d5621ca8afccf988201f47f6d90803d7602`  
		Last Modified: Tue, 20 Sep 2022 21:19:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a5bec081c2ffab9cf55ad27265d196049831a31636b189898d381b83f4ec8e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16766479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8be559ac2b0c6ab85c56fba8d461e2ad32cefd34996ede58394d39e970d6e80`
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
# Tue, 20 Sep 2022 20:49:16 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 20:49:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='c05515dd332aa2ef1d50ff7285118deb31aabed336efb8234aaaafe531d0a4525488deffdccd50a20bb9688d4df15464a7d3642956975942528b1705f7811b08' ;; 		armhf)   binArch='armv6'; checksum='e40d557c5c36ae5fe956e1906c3e967f925daf115347188c19b47b118dc7d2c967e8caa8e8a7604a5474114d33552611c85b9135b0ea2c08045635dc6c2a0316' ;; 		armv7)   binArch='armv7'; checksum='6ce633b30541767f93fb1115ab34448d6275856e3dc9fcc31a7ea0472f322838057d23274116181bb15558caac41ddeab89f156880143769485f0b6870afecdb' ;; 		aarch64) binArch='arm64'; checksum='6c7aed21dceec7532ec39c4fa79ba7df6e15cfb9c8802244893de8c6b1998eef79a54810bed271e962c5546be482d6dcc20cbeb9773d23920abbf75694afcbe1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='abd734031a318d69296e0e8776b62267466cbdbc994079db4d9615d15ce79a2369a58317a6d812fe0979bcfe447b15dc5a53f1bad97e9e9b2b4af69a331da17d' ;; 		s390x)   binArch='s390x'; checksum='b727ba39563709f5f53f026e96e6361d0649b9bb7a151f5ecb46b4c1652664516999c708d65b96366b87730ced97b826256fad2ac04db171be893dde815388be' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 20 Sep 2022 20:49:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Sep 2022 20:49:19 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 20 Sep 2022 20:49:19 GMT
ENV XDG_DATA_HOME=/data
# Tue, 20 Sep 2022 20:49:19 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 20:49:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 20:49:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 20:49:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 20:49:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 20:49:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 20:49:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 20:49:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 20:49:20 GMT
EXPOSE 80
# Tue, 20 Sep 2022 20:49:20 GMT
EXPOSE 443
# Tue, 20 Sep 2022 20:49:20 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 20:49:20 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 20:49:20 GMT
WORKDIR /srv
# Tue, 20 Sep 2022 20:49:21 GMT
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
	-	`sha256:b62bfdcbde37976f9ed8ab9251e9239682cddd538ac150fe5a5e2445efd03fd5`  
		Last Modified: Tue, 20 Sep 2022 20:50:06 GMT  
		Size: 13.8 MB (13842059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dff61bcc7ec0f9b88a513cf292d8b9a8d229c128d6f606eedff9938c9fedd71`  
		Last Modified: Tue, 20 Sep 2022 20:50:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:251564057371a69428947acd9726c7eefebe8bb5c13504c235ca3a56645ddaed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16546577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0dc1544841490217acbd4a5ab1f31c0cd37026b6b1763fd6a448ed490929c9`
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
# Tue, 20 Sep 2022 20:57:19 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 20:57:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='c05515dd332aa2ef1d50ff7285118deb31aabed336efb8234aaaafe531d0a4525488deffdccd50a20bb9688d4df15464a7d3642956975942528b1705f7811b08' ;; 		armhf)   binArch='armv6'; checksum='e40d557c5c36ae5fe956e1906c3e967f925daf115347188c19b47b118dc7d2c967e8caa8e8a7604a5474114d33552611c85b9135b0ea2c08045635dc6c2a0316' ;; 		armv7)   binArch='armv7'; checksum='6ce633b30541767f93fb1115ab34448d6275856e3dc9fcc31a7ea0472f322838057d23274116181bb15558caac41ddeab89f156880143769485f0b6870afecdb' ;; 		aarch64) binArch='arm64'; checksum='6c7aed21dceec7532ec39c4fa79ba7df6e15cfb9c8802244893de8c6b1998eef79a54810bed271e962c5546be482d6dcc20cbeb9773d23920abbf75694afcbe1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='abd734031a318d69296e0e8776b62267466cbdbc994079db4d9615d15ce79a2369a58317a6d812fe0979bcfe447b15dc5a53f1bad97e9e9b2b4af69a331da17d' ;; 		s390x)   binArch='s390x'; checksum='b727ba39563709f5f53f026e96e6361d0649b9bb7a151f5ecb46b4c1652664516999c708d65b96366b87730ced97b826256fad2ac04db171be893dde815388be' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 20 Sep 2022 20:57:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Sep 2022 20:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 20 Sep 2022 20:57:22 GMT
ENV XDG_DATA_HOME=/data
# Tue, 20 Sep 2022 20:57:22 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 20:57:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 20:57:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 20:57:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 20:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 20:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 20:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 20:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 20:57:23 GMT
EXPOSE 80
# Tue, 20 Sep 2022 20:57:23 GMT
EXPOSE 443
# Tue, 20 Sep 2022 20:57:24 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 20:57:24 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 20:57:24 GMT
WORKDIR /srv
# Tue, 20 Sep 2022 20:57:24 GMT
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
	-	`sha256:5ddec397395514d027e9c6468530ec459a8decc2097380ef0928cc4c5e900f27`  
		Last Modified: Tue, 20 Sep 2022 20:58:10 GMT  
		Size: 13.8 MB (13819918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf848c46ead06f524b2677c0d8db963ac98016b619aae5ff173cb6a3a4b92a8`  
		Last Modified: Tue, 20 Sep 2022 20:58:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:398623cd8e4d1084a1a4fa3ee53f226d3f1e4be028b7a4e1ef782f02afdd99d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16211068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0203ffb3530a2a3999d8ba600447ab12c3e33e0913dbad0815752d8e93ab9fbc`
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
# Tue, 20 Sep 2022 20:41:32 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 20:41:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='c05515dd332aa2ef1d50ff7285118deb31aabed336efb8234aaaafe531d0a4525488deffdccd50a20bb9688d4df15464a7d3642956975942528b1705f7811b08' ;; 		armhf)   binArch='armv6'; checksum='e40d557c5c36ae5fe956e1906c3e967f925daf115347188c19b47b118dc7d2c967e8caa8e8a7604a5474114d33552611c85b9135b0ea2c08045635dc6c2a0316' ;; 		armv7)   binArch='armv7'; checksum='6ce633b30541767f93fb1115ab34448d6275856e3dc9fcc31a7ea0472f322838057d23274116181bb15558caac41ddeab89f156880143769485f0b6870afecdb' ;; 		aarch64) binArch='arm64'; checksum='6c7aed21dceec7532ec39c4fa79ba7df6e15cfb9c8802244893de8c6b1998eef79a54810bed271e962c5546be482d6dcc20cbeb9773d23920abbf75694afcbe1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='abd734031a318d69296e0e8776b62267466cbdbc994079db4d9615d15ce79a2369a58317a6d812fe0979bcfe447b15dc5a53f1bad97e9e9b2b4af69a331da17d' ;; 		s390x)   binArch='s390x'; checksum='b727ba39563709f5f53f026e96e6361d0649b9bb7a151f5ecb46b4c1652664516999c708d65b96366b87730ced97b826256fad2ac04db171be893dde815388be' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 20 Sep 2022 20:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Sep 2022 20:41:37 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 20 Sep 2022 20:41:38 GMT
ENV XDG_DATA_HOME=/data
# Tue, 20 Sep 2022 20:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 20:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 20:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 20:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 20:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 20:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 20:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 20:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 20:41:47 GMT
EXPOSE 80
# Tue, 20 Sep 2022 20:41:48 GMT
EXPOSE 443
# Tue, 20 Sep 2022 20:41:49 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 20:41:50 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 20:41:51 GMT
WORKDIR /srv
# Tue, 20 Sep 2022 20:41:52 GMT
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
	-	`sha256:d64229b3f616b23cfaa960ea2cf99414459ab2b6d32e4269a2e246ce897e72f5`  
		Last Modified: Tue, 20 Sep 2022 20:42:36 GMT  
		Size: 13.2 MB (13193199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031b0050e7ad64612adba5473db0c853e96003c7fef5a4bafec61c1e6a018cb8`  
		Last Modified: Tue, 20 Sep 2022 20:42:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:86b53e5b718ce96ba8dfed3ac739c50d8c48d5a9d045ab72db0a59ff445b9849
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15965324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2068223e19cc5d0ee21c120346a11f524e1f55087c1f1ddea7c4e8f88c9bf90a`
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
# Tue, 20 Sep 2022 21:16:20 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 21:16:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='c05515dd332aa2ef1d50ff7285118deb31aabed336efb8234aaaafe531d0a4525488deffdccd50a20bb9688d4df15464a7d3642956975942528b1705f7811b08' ;; 		armhf)   binArch='armv6'; checksum='e40d557c5c36ae5fe956e1906c3e967f925daf115347188c19b47b118dc7d2c967e8caa8e8a7604a5474114d33552611c85b9135b0ea2c08045635dc6c2a0316' ;; 		armv7)   binArch='armv7'; checksum='6ce633b30541767f93fb1115ab34448d6275856e3dc9fcc31a7ea0472f322838057d23274116181bb15558caac41ddeab89f156880143769485f0b6870afecdb' ;; 		aarch64) binArch='arm64'; checksum='6c7aed21dceec7532ec39c4fa79ba7df6e15cfb9c8802244893de8c6b1998eef79a54810bed271e962c5546be482d6dcc20cbeb9773d23920abbf75694afcbe1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='abd734031a318d69296e0e8776b62267466cbdbc994079db4d9615d15ce79a2369a58317a6d812fe0979bcfe447b15dc5a53f1bad97e9e9b2b4af69a331da17d' ;; 		s390x)   binArch='s390x'; checksum='b727ba39563709f5f53f026e96e6361d0649b9bb7a151f5ecb46b4c1652664516999c708d65b96366b87730ced97b826256fad2ac04db171be893dde815388be' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 20 Sep 2022 21:16:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Sep 2022 21:16:26 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 20 Sep 2022 21:16:26 GMT
ENV XDG_DATA_HOME=/data
# Tue, 20 Sep 2022 21:16:26 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 21:16:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 21:16:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 21:16:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 21:16:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 21:16:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 21:16:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 21:16:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 21:16:28 GMT
EXPOSE 80
# Tue, 20 Sep 2022 21:16:29 GMT
EXPOSE 443
# Tue, 20 Sep 2022 21:16:29 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 21:16:29 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 21:16:30 GMT
WORKDIR /srv
# Tue, 20 Sep 2022 21:16:30 GMT
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
	-	`sha256:aa32d116b14f15b178f13e49de164d470c152d6ba690fc9841132102af43d66c`  
		Last Modified: Tue, 20 Sep 2022 21:17:15 GMT  
		Size: 12.8 MB (12849510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913fcd4ca852c1146be080945e9e9ff041382fac17af6daf049c70c59ad4e9b2`  
		Last Modified: Tue, 20 Sep 2022 21:17:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:07db4261c79474418221538b52dca377b8f681463b0e6e75966a883f73c975bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16898237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee2687fba12c0a5b663672c613c1cc1f5cb2fc60fe96f86e698f8615aaa8ff2`
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
# Tue, 20 Sep 2022 20:41:28 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 20:41:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='c05515dd332aa2ef1d50ff7285118deb31aabed336efb8234aaaafe531d0a4525488deffdccd50a20bb9688d4df15464a7d3642956975942528b1705f7811b08' ;; 		armhf)   binArch='armv6'; checksum='e40d557c5c36ae5fe956e1906c3e967f925daf115347188c19b47b118dc7d2c967e8caa8e8a7604a5474114d33552611c85b9135b0ea2c08045635dc6c2a0316' ;; 		armv7)   binArch='armv7'; checksum='6ce633b30541767f93fb1115ab34448d6275856e3dc9fcc31a7ea0472f322838057d23274116181bb15558caac41ddeab89f156880143769485f0b6870afecdb' ;; 		aarch64) binArch='arm64'; checksum='6c7aed21dceec7532ec39c4fa79ba7df6e15cfb9c8802244893de8c6b1998eef79a54810bed271e962c5546be482d6dcc20cbeb9773d23920abbf75694afcbe1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='abd734031a318d69296e0e8776b62267466cbdbc994079db4d9615d15ce79a2369a58317a6d812fe0979bcfe447b15dc5a53f1bad97e9e9b2b4af69a331da17d' ;; 		s390x)   binArch='s390x'; checksum='b727ba39563709f5f53f026e96e6361d0649b9bb7a151f5ecb46b4c1652664516999c708d65b96366b87730ced97b826256fad2ac04db171be893dde815388be' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 20 Sep 2022 20:41:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 20 Sep 2022 20:41:38 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 20 Sep 2022 20:41:38 GMT
ENV XDG_DATA_HOME=/data
# Tue, 20 Sep 2022 20:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 20:41:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 20:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 20:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 20:41:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 20:41:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 20:41:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 20:41:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 20:41:43 GMT
EXPOSE 80
# Tue, 20 Sep 2022 20:41:43 GMT
EXPOSE 443
# Tue, 20 Sep 2022 20:41:44 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 20:41:44 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 20:41:44 GMT
WORKDIR /srv
# Tue, 20 Sep 2022 20:41:45 GMT
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
	-	`sha256:e99b8d0ad0c5bda305ed34c6b089bf8afb5800e219fb4b191fbadb9c98068a9b`  
		Last Modified: Tue, 20 Sep 2022 20:42:41 GMT  
		Size: 14.0 MB (13996915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031b0050e7ad64612adba5473db0c853e96003c7fef5a4bafec61c1e6a018cb8`  
		Last Modified: Tue, 20 Sep 2022 20:42:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.3406; amd64

```console
$ docker pull caddy@sha256:d7db9b1b3cdab1567bf91ad1f3b49525813d2a01171c5887ad5b9025081d9eb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2719160168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7683f48122d450dec80a02a03dab974285800188fd6984e74c4f490274213957`
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
# Tue, 20 Sep 2022 21:15:49 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 21:17:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('49582519293819fd4086540aa83428f75af7074882056b6cbe7ab29038f11587f9b6ea2bd68de583e4e99e7afb5bd42ea943e81065a1dc0b5f0b3057f7a0da0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 20 Sep 2022 21:17:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 20 Sep 2022 21:17:13 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 20 Sep 2022 21:17:14 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 21:17:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 21:17:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 21:17:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 21:17:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 21:17:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 21:17:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 21:17:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 21:17:21 GMT
EXPOSE 80
# Tue, 20 Sep 2022 21:17:22 GMT
EXPOSE 443
# Tue, 20 Sep 2022 21:17:23 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 21:17:24 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 21:18:14 GMT
RUN caddy version
# Tue, 20 Sep 2022 21:18:15 GMT
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
	-	`sha256:c321b986d79e251e57d07601b1c55fa13d2b45ef9de8768ddd9c3cadf89b5852`  
		Last Modified: Tue, 20 Sep 2022 21:22:08 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebf735c6fd9e641b384edbfe6ba5ceb05307d107b7372cef5dedafaebb69506`  
		Last Modified: Tue, 20 Sep 2022 21:22:11 GMT  
		Size: 14.9 MB (14904011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b3aeef135416d6c6356531b8eaccd78775b16fcaa39e74906684285a19c21`  
		Last Modified: Tue, 20 Sep 2022 21:22:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75af89279a5fa4169d839cc86b46b4637eecdbd7dd41f69bbd7d8c1f5a39cd20`  
		Last Modified: Tue, 20 Sep 2022 21:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dae98dc0855ebe2c41992478fe662d776b39954dcf97e87b78e6202a07d10df`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524294a3cdce5ce2e8ab0086f1e8151f01a958c7a435af7f2721f3de00908b99`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5deb16e98516130995b20182b32b6320eee2a629d6c2336a51fa5c6d28f8fe90`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6926d330fbe8a23a3cff8957075f0cca0e889082baa27fd52c1070f50decbd`  
		Last Modified: Tue, 20 Sep 2022 21:22:06 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caa7a22d1f59d8d1a3d0b6ac4fa4aa729c7478491ee8cc124be7d7ba7097deb`  
		Last Modified: Tue, 20 Sep 2022 21:22:04 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea66fc4101419cb9eba83238cf945eecca732dbd52f2184b6e2b967f92d49f3f`  
		Last Modified: Tue, 20 Sep 2022 21:22:04 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df966808bb1c7e3b916a530158feefcfce8699034d9c07c7b9ad3c5f50aac6b3`  
		Last Modified: Tue, 20 Sep 2022 21:22:03 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c257d1dd36c1f128bb7805c57ef3c339189749d51e663771e4a8d3b7d8437390`  
		Last Modified: Tue, 20 Sep 2022 21:22:03 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7c526b2d38f043453b8220aefaeee679e3ff7ae00b2e55fbd5218a12e4333`  
		Last Modified: Tue, 20 Sep 2022 21:22:03 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c8e0ffe60e71db7689f6f05bb71bc3d81192a83166bddf2b57445b6459a5e`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab8b8dbcb7997076b6b7f02563628c13f0ad49a0dedd0788c0cb25d9df49564`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bc4d651137a0c053a4c2a929ce35948c90e2ec719b7a434a4e23cd45ff2db7`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba74362d5c5ebd167aaaeafb147886f6089088c081a52fa88939414a38e49778`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 307.7 KB (307722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b417cb891c81d0327c5a5fec64ea647390aca9869e325a1bf78f08c1b21e3d9e`  
		Last Modified: Tue, 20 Sep 2022 21:22:01 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1006; amd64

```console
$ docker pull caddy@sha256:dc4ee7e519ed48896bf323f60b79341aa92f2b02671a91c6007dbf0912bdbb54
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363004397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffee00981fb92f0732b4ae4de1ef5bc1e278ddc860a5473b163ad5bd532ad7d2`
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
# Tue, 20 Sep 2022 21:18:37 GMT
ENV CADDY_VERSION=v2.6.0
# Tue, 20 Sep 2022 21:19:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.0/caddy_2.6.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('49582519293819fd4086540aa83428f75af7074882056b6cbe7ab29038f11587f9b6ea2bd68de583e4e99e7afb5bd42ea943e81065a1dc0b5f0b3057f7a0da0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 20 Sep 2022 21:19:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 20 Sep 2022 21:19:11 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 20 Sep 2022 21:19:12 GMT
LABEL org.opencontainers.image.version=v2.6.0
# Tue, 20 Sep 2022 21:19:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 20 Sep 2022 21:19:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 20 Sep 2022 21:19:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 20 Sep 2022 21:19:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 20 Sep 2022 21:19:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 20 Sep 2022 21:19:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 20 Sep 2022 21:19:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 20 Sep 2022 21:19:19 GMT
EXPOSE 80
# Tue, 20 Sep 2022 21:19:20 GMT
EXPOSE 443
# Tue, 20 Sep 2022 21:19:21 GMT
EXPOSE 443/udp
# Tue, 20 Sep 2022 21:19:21 GMT
EXPOSE 2019
# Tue, 20 Sep 2022 21:19:37 GMT
RUN caddy version
# Tue, 20 Sep 2022 21:19:38 GMT
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
	-	`sha256:9a9c4e9ef3240230369006cd96a01ebf2122f9a02d2629611a2596cd1b2aa65d`  
		Last Modified: Tue, 20 Sep 2022 21:22:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d67752bfbf9c5f6590ada30bfef8117dfaa1c7131eaf6dd9fe1550adb92e8d`  
		Last Modified: Tue, 20 Sep 2022 21:22:36 GMT  
		Size: 15.1 MB (15098856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3834bb5e4908dbbcec6c6ee9360c374df86e895c251843dc024649599050d267`  
		Last Modified: Tue, 20 Sep 2022 21:22:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a77eef44e97a57e420415da1d41fab986f3c74f9ce434e345015b5ed8c1f16`  
		Last Modified: Tue, 20 Sep 2022 21:22:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8710898e66657abdc81c9dd22b7a2db1d2b1edb8c39a090af592ffcfcd3f2401`  
		Last Modified: Tue, 20 Sep 2022 21:22:30 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7309b13f447c9a18a51f88bab5049962910858d7bd97e24a0a05436abb73ca52`  
		Last Modified: Tue, 20 Sep 2022 21:22:30 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b0f3b9d781303a6839d67a52fe9f5b78eea9555e609f6e701e7309a8c161cf`  
		Last Modified: Tue, 20 Sep 2022 21:22:30 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08a308260ceb21be52c3b8b30c806f982f7833beea2024ae92881c21dbb079c`  
		Last Modified: Tue, 20 Sep 2022 21:22:30 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72340a238d4fdb5cfcbf2a8fe13b74f3219eb9e69be47e31641bebe3e3f6789`  
		Last Modified: Tue, 20 Sep 2022 21:22:28 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7acc54d37c6fa412dad4dfcd1ea8ae743030a9800cc35e716b048177be7434`  
		Last Modified: Tue, 20 Sep 2022 21:22:28 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43d3bbc94dae0fae0669d4f82d0928927d78793e5ee481ad70bb71e77782665`  
		Last Modified: Tue, 20 Sep 2022 21:22:28 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20758e7b9e978cd5164e4c3e30ae4b08b70ebb949dd38ca20d9979336f0e7b31`  
		Last Modified: Tue, 20 Sep 2022 21:22:28 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d1ba2e6cf728a7f657b1bad78c3960831c5938d30e6c2fde295ecd602adc3a`  
		Last Modified: Tue, 20 Sep 2022 21:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44c02ace8b9c28c4cdf2cecd67d6c9ab086dc0599d76d3355d1067fbe2c11e`  
		Last Modified: Tue, 20 Sep 2022 21:22:25 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8117de42949643daf5932991176e82ed304a5018d7f0da0c7ddbadef4c89243`  
		Last Modified: Tue, 20 Sep 2022 21:22:26 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b4e182952d8d7f9466076264a992271cb0ad6ffce5fe3357dd4c6ef1c0577`  
		Last Modified: Tue, 20 Sep 2022 21:22:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b706ae4bf39e00022b108e391a58f738e4680fe2ee68cd491da15c1f3ae64342`  
		Last Modified: Tue, 20 Sep 2022 21:22:26 GMT  
		Size: 332.2 KB (332201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7075dd1edbdec598cea20208856a0d01169dba8e31d64175dae0cf35620026a`  
		Last Modified: Tue, 20 Sep 2022 21:22:26 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
