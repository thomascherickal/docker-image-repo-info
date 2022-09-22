## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:8216dfa3979a63f3a30829de12ac71c178ad8025f434f2c61e9d3be6bbc7761b
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

### `caddy:2-alpine` - linux; ppc64le

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
