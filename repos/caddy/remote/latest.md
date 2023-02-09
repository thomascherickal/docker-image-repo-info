## `caddy:latest`

```console
$ docker pull caddy@sha256:fcf71b95acbfbf3d40f97d731db2b4b177193a0c7880d60c48d6389308053042
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:latest` - linux; amd64

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

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:24991b01e57808156c167d5050346e4fb47c3cc45f4aff8ae2891c3d24f7be3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16574982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f36376cee92f035a8b6f26466ed7cd4187facca859d79e1ed1d31cdcfadc81`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Wed, 08 Feb 2023 23:49:22 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Feb 2023 23:49:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Feb 2023 23:49:24 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Feb 2023 23:49:29 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Feb 2023 23:49:30 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Feb 2023 23:49:30 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Wed, 08 Feb 2023 23:49:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Feb 2023 23:49:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Feb 2023 23:49:31 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Feb 2023 23:49:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Feb 2023 23:49:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Feb 2023 23:49:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Feb 2023 23:49:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Feb 2023 23:49:32 GMT
EXPOSE 80
# Wed, 08 Feb 2023 23:49:32 GMT
EXPOSE 443
# Wed, 08 Feb 2023 23:49:33 GMT
EXPOSE 443/udp
# Wed, 08 Feb 2023 23:49:33 GMT
EXPOSE 2019
# Wed, 08 Feb 2023 23:49:33 GMT
WORKDIR /srv
# Wed, 08 Feb 2023 23:49:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1732a0e7cbbbf709a1d596a3995a789db67dff4c4b693c8222b58c485c38e98d`  
		Last Modified: Wed, 08 Feb 2023 23:50:37 GMT  
		Size: 345.8 KB (345815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811dd897848be6b71f3ee5390cb361f66bd9f7ff542698104318ebf8ca925dfb`  
		Last Modified: Wed, 08 Feb 2023 23:50:37 GMT  
		Size: 7.5 KB (7477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f4c9b24ea6404454ae52e30ff9c4bd73f66aa1c44eddb521bee8b0c2dc252f`  
		Last Modified: Wed, 08 Feb 2023 23:50:39 GMT  
		Size: 13.6 MB (13606585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a12f8b257edf723252fe4d7904cd7da6427f0143cd91fd8f1c66d4238d8fc3b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16360408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e339ad4e3cdbcdb2b56b0f159d20385f1b8ba9df46bd139c4648267b3ed55454`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Wed, 08 Feb 2023 23:57:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Feb 2023 23:57:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Feb 2023 23:57:29 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Feb 2023 23:57:32 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Feb 2023 23:57:32 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Feb 2023 23:57:32 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Wed, 08 Feb 2023 23:57:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Feb 2023 23:57:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Feb 2023 23:57:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 80
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 443
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 443/udp
# Wed, 08 Feb 2023 23:57:33 GMT
EXPOSE 2019
# Wed, 08 Feb 2023 23:57:34 GMT
WORKDIR /srv
# Wed, 08 Feb 2023 23:57:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a12332fdf16ce73aea4764330485716ca48d192a121a2fd401dc2c0b39218f`  
		Last Modified: Wed, 08 Feb 2023 23:58:28 GMT  
		Size: 342.6 KB (342593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b77a300a01493d7a60c76bceedba787157bd56b11597beb662bdb689c2ad2a`  
		Last Modified: Wed, 08 Feb 2023 23:58:28 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79d8027362d8d140a1b1f357f0eeb8db4538ad6953141f1be740c8f251f1f7`  
		Last Modified: Wed, 08 Feb 2023 23:58:31 GMT  
		Size: 13.6 MB (13591547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
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
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
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
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:ee3ae0f0030f5ce972d9542650e4d637e0ef94e01ae281191f3feaacceb90a72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16784652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6256db384255ae9f0b4b233b101f88c3e12d88e57c7584b02a70f5271c942254`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Wed, 08 Feb 2023 23:41:38 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Feb 2023 23:41:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Feb 2023 23:41:40 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Feb 2023 23:41:45 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Feb 2023 23:41:46 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Feb 2023 23:41:46 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Wed, 08 Feb 2023 23:41:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Feb 2023 23:41:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Feb 2023 23:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Feb 2023 23:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Feb 2023 23:41:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Feb 2023 23:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Feb 2023 23:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Feb 2023 23:41:48 GMT
EXPOSE 80
# Wed, 08 Feb 2023 23:41:48 GMT
EXPOSE 443
# Wed, 08 Feb 2023 23:41:49 GMT
EXPOSE 443/udp
# Wed, 08 Feb 2023 23:41:49 GMT
EXPOSE 2019
# Wed, 08 Feb 2023 23:41:49 GMT
WORKDIR /srv
# Wed, 08 Feb 2023 23:41:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bb3bec7204cd5466e4667b10196adcfbbb83ef447217c88dccdeefcfab7d7d`  
		Last Modified: Wed, 08 Feb 2023 23:42:38 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae9a4c1271b494319847404abfdceb2c942858a3eab912684995fa22e9e2606`  
		Last Modified: Wed, 08 Feb 2023 23:42:38 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c451db11e6ce6423fc269256710f0dd06f5dc105c0b365de42f9f915ad1a95`  
		Last Modified: Wed, 08 Feb 2023 23:42:40 GMT  
		Size: 13.8 MB (13833174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
