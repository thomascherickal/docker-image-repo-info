## `caddy:alpine`

```console
$ docker pull caddy@sha256:627b79a174491107498b3d22a0eef08b144f670f9c9d973e505edf7fe4e08ed3
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
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
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
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
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
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
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
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
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
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
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
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
