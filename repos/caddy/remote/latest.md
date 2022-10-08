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
