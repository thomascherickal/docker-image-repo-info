## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:4fd05702a7c12e4266b22496369efc69f988953194f702be82daa764d5540079
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
$ docker pull caddy@sha256:c0cb0c7ff63937fc641664895e1844666baf2f00eed688237f2e093a9a04a6a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a399f1211b45b8dbf10005ab3deec678552c502ac66a63ea3027a2ac30051414`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:38:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 02:38:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 02:38:22 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 02:38:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 02:38:29 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 02:38:29 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 02:38:30 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 02:38:30 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 02:38:30 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 02:38:31 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 02:38:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 02:38:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 02:38:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 02:38:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 02:38:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 02:38:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 02:38:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 02:38:34 GMT
EXPOSE 80
# Fri, 26 Mar 2021 02:38:34 GMT
EXPOSE 443
# Fri, 26 Mar 2021 02:38:35 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 02:38:35 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 02:38:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86cfaea3777414001ca8c36d3fb1c35e31ab133ef9edc3c047ae288ef70eb04`  
		Last Modified: Fri, 26 Mar 2021 02:39:44 GMT  
		Size: 300.0 KB (300017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b3ec4462bfd2b0286ff34909a730ba5f0ac56724d79f281d8837cb9a21492`  
		Last Modified: Fri, 26 Mar 2021 02:39:44 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0074ab5b262dbef2b99e9b03ce56382bb7b5c994d4015b1d035f954f05249a26`  
		Last Modified: Fri, 26 Mar 2021 02:39:47 GMT  
		Size: 11.6 MB (11622386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3482ef241eb9ce7284f69e549fc2ae9718230317834f0476186ef15f535af35a`  
		Last Modified: Fri, 26 Mar 2021 02:39:44 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c3b7953b6327122af0855af37c04ae19d294d00fff1f24654db9d7d8be6d8972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13855742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c25b74318718ca079aa92e61e23122ed39a1b579391956e16d4663eb255aab2b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:43 GMT
ADD file:65a3462a527f49c8c625927be6b8b57b4257c8cc37d685055a1f183d76c68920 in / 
# Thu, 25 Mar 2021 22:50:47 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:08:19 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 00:08:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 00:08:26 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 00:08:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 00:08:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:08:40 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 00:08:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 00:08:44 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 00:08:47 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 00:08:50 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 00:08:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 00:08:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 00:08:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 00:08:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 00:08:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 00:08:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 00:09:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 00:09:01 GMT
EXPOSE 80
# Fri, 26 Mar 2021 00:09:03 GMT
EXPOSE 443
# Fri, 26 Mar 2021 00:09:04 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 00:09:06 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 00:09:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:181a1446f0acaaa0871cec07aba4f733041f2d80ffbe01b19df43fe005df29f3`  
		Last Modified: Thu, 25 Mar 2021 22:55:06 GMT  
		Size: 2.6 MB (2604815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15160e7d182b159f41c99bec8708c0ec86e77aaa49f040ea44dd42f6c58ebfe`  
		Last Modified: Fri, 26 Mar 2021 00:12:45 GMT  
		Size: 300.1 KB (300118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899e34fea964a2467d15dc923f0936b8db1b8382e56992f4bb0dcf00e5a16b5a`  
		Last Modified: Fri, 26 Mar 2021 00:12:45 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92447db2f519898b5bb6dbb4a6ebcaf799affeb30c4247dca33ae4a13461521c`  
		Last Modified: Fri, 26 Mar 2021 00:12:49 GMT  
		Size: 10.9 MB (10944823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efe14174f225a5ab672dadf00353b1530ca172dc38e1d93dfcf8f324015aa7e`  
		Last Modified: Fri, 26 Mar 2021 00:12:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0afebb6789caf77d5b93736c2fc6e69faea87ac5b32658167fd537555d609d04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13638861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb75b72a916033f3c532848aeefdc4b0d0dbf476a45f102830ecc99326f2b95b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:06:14 GMT
ADD file:09312e8d8073093cdfa852f8a73713903ec5022b963fe0413feb08af5c98721b in / 
# Thu, 25 Mar 2021 22:06:16 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:12:28 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 26 Mar 2021 00:12:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Fri, 26 Mar 2021 00:12:34 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 26 Mar 2021 00:12:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Mar 2021 00:12:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 00:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Mar 2021 00:12:48 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Mar 2021 00:12:50 GMT
VOLUME [/config]
# Fri, 26 Mar 2021 00:12:51 GMT
VOLUME [/data]
# Fri, 26 Mar 2021 00:12:53 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Fri, 26 Mar 2021 00:12:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Mar 2021 00:12:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Mar 2021 00:12:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Mar 2021 00:13:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Mar 2021 00:13:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Mar 2021 00:13:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Mar 2021 00:13:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Mar 2021 00:13:11 GMT
EXPOSE 80
# Fri, 26 Mar 2021 00:13:14 GMT
EXPOSE 443
# Fri, 26 Mar 2021 00:13:16 GMT
EXPOSE 2019
# Fri, 26 Mar 2021 00:13:18 GMT
WORKDIR /srv
# Fri, 26 Mar 2021 00:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1d60ece6104ddbfa31c28af7c5c9c14957b3b271ea6f7edac14f84f4cd8c5fa9`  
		Last Modified: Thu, 25 Mar 2021 22:07:33 GMT  
		Size: 2.4 MB (2408322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8662621fb9d12eafc80b7c654846271ac59600d85674edd7b658ce07900664d3`  
		Last Modified: Fri, 26 Mar 2021 00:15:23 GMT  
		Size: 299.2 KB (299210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3b14c2dc5ed630914742e70417caa422ffb0379e67b8fe1c12a5cd5d6879a5`  
		Last Modified: Fri, 26 Mar 2021 00:15:23 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10382462a35e453a671fd3bce5a9df6e178f93fd546f0dafe8774e6d622937e6`  
		Last Modified: Fri, 26 Mar 2021 00:15:29 GMT  
		Size: 10.9 MB (10925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d778116296d33a2036facfe0f0917c74aeb3efbc228e3a8929fd0b14b2867ff1`  
		Last Modified: Fri, 26 Mar 2021 00:15:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2760e78ed4694a84bd2d6c9f8757e0f2eef516d52254f98277005e3332940156
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13614976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb1c06d0b71ebdf93ccd671ded898dbc05fb92605aaa2e613a00c690c63f307`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:31:31 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 25 Mar 2021 23:31:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 25 Mar 2021 23:32:08 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Mar 2021 23:32:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 25 Mar 2021 23:32:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 25 Mar 2021 23:33:02 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 25 Mar 2021 23:33:13 GMT
ENV XDG_DATA_HOME=/data
# Thu, 25 Mar 2021 23:33:20 GMT
VOLUME [/config]
# Thu, 25 Mar 2021 23:33:35 GMT
VOLUME [/data]
# Thu, 25 Mar 2021 23:33:41 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 25 Mar 2021 23:33:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 25 Mar 2021 23:33:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 25 Mar 2021 23:33:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 25 Mar 2021 23:33:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 25 Mar 2021 23:33:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 25 Mar 2021 23:34:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 25 Mar 2021 23:34:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 25 Mar 2021 23:34:38 GMT
EXPOSE 80
# Thu, 25 Mar 2021 23:35:00 GMT
EXPOSE 443
# Thu, 25 Mar 2021 23:35:06 GMT
EXPOSE 2019
# Thu, 25 Mar 2021 23:35:19 GMT
WORKDIR /srv
# Thu, 25 Mar 2021 23:35:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18097d4c9638c3cd9be2c7e06cf74879d0c24caa73501e2adfa40b02ec79e261`  
		Last Modified: Thu, 25 Mar 2021 23:42:19 GMT  
		Size: 300.3 KB (300322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8feda3f9171d8b727a6d38d73439a098d5e367e1e7346b0d346e7c09e26cec`  
		Last Modified: Thu, 25 Mar 2021 23:42:19 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60fde45401cbb316e0c5b208967fc883da8992e8b892a574bcb4e69ba7d7e6e`  
		Last Modified: Thu, 25 Mar 2021 23:42:26 GMT  
		Size: 10.6 MB (10598976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f235d25412984912e2016f077ff2c324bbfec9fcfc7051d30f549c5187904f32`  
		Last Modified: Thu, 25 Mar 2021 23:42:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:835954456f4b23bc0438b0423cfb25b19d1f184d85c44e7d50483c98c1bdb237
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13355613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f32f89e24ae18bc58ff2f9474e23a0240dcf374e6f2ff1f6f01dbde7895883b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:02:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 24 Feb 2021 21:02:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 24 Feb 2021 21:02:42 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 24 Feb 2021 21:02:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 24 Feb 2021 21:03:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:03:16 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 24 Feb 2021 21:03:21 GMT
ENV XDG_DATA_HOME=/data
# Wed, 24 Feb 2021 21:03:28 GMT
VOLUME [/config]
# Wed, 24 Feb 2021 21:03:33 GMT
VOLUME [/data]
# Wed, 24 Feb 2021 21:03:37 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 24 Feb 2021 21:03:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 24 Feb 2021 21:03:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 24 Feb 2021 21:03:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 24 Feb 2021 21:03:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 24 Feb 2021 21:04:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 24 Feb 2021 21:04:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 24 Feb 2021 21:04:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 24 Feb 2021 21:04:13 GMT
EXPOSE 80
# Wed, 24 Feb 2021 21:04:17 GMT
EXPOSE 443
# Wed, 24 Feb 2021 21:04:22 GMT
EXPOSE 2019
# Wed, 24 Feb 2021 21:04:28 GMT
WORKDIR /srv
# Wed, 24 Feb 2021 21:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9864d4f9ffa98b896ad863ec705c2a2bce2aa8691403eecce7790d467de7e89`  
		Last Modified: Wed, 24 Feb 2021 21:05:09 GMT  
		Size: 302.3 KB (302341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c72b4f216ba67dc77214d3ec8d53e95b9f4a7989eb80b52621fcf35941362dc`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bd52028343039b1f04dfc295f0a8c69da2291e8821a937274bcab1d94e2c5`  
		Last Modified: Wed, 24 Feb 2021 21:05:12 GMT  
		Size: 10.2 MB (10241391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf4197b2f1cc35b12da368fd4455bab68c9d6034ce3d778ae2d146d0b111ec`  
		Last Modified: Wed, 24 Feb 2021 21:05:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e343f581e0e3e2df11f6a26d4cb7588f61ba912fb70329c2dd53d221203273cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14145971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a04dbac2b5dc7e783218e3324502b4b291522838759f68e86f16b6020028abc5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:39 GMT
ADD file:12766b6fe7c37292d91bd1469b27dc9fb362e3109e9b3f377cff030bc0ca5386 in / 
# Thu, 25 Mar 2021 22:41:39 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 22:59:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 25 Mar 2021 22:59:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Thu, 25 Mar 2021 22:59:05 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 25 Mar 2021 22:59:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 25 Mar 2021 22:59:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 25 Mar 2021 22:59:08 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 25 Mar 2021 22:59:09 GMT
ENV XDG_DATA_HOME=/data
# Thu, 25 Mar 2021 22:59:09 GMT
VOLUME [/config]
# Thu, 25 Mar 2021 22:59:09 GMT
VOLUME [/data]
# Thu, 25 Mar 2021 22:59:09 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Thu, 25 Mar 2021 22:59:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 25 Mar 2021 22:59:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 25 Mar 2021 22:59:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 25 Mar 2021 22:59:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 25 Mar 2021 22:59:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 25 Mar 2021 22:59:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 25 Mar 2021 22:59:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 25 Mar 2021 22:59:11 GMT
EXPOSE 80
# Thu, 25 Mar 2021 22:59:11 GMT
EXPOSE 443
# Thu, 25 Mar 2021 22:59:11 GMT
EXPOSE 2019
# Thu, 25 Mar 2021 22:59:12 GMT
WORKDIR /srv
# Thu, 25 Mar 2021 22:59:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:be2cdf7cbb6a1aec476a957daaae210624b2b112c20f27f55bbcf2bdc74db281`  
		Last Modified: Thu, 25 Mar 2021 22:42:19 GMT  
		Size: 2.6 MB (2567457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd30cda4b096d348f0713fa511ceedfb697fcd625e3063cdc8144c43aef0901`  
		Last Modified: Thu, 25 Mar 2021 22:59:56 GMT  
		Size: 300.5 KB (300467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1eeb04394ba8dc2eb7acd8b4ca1dd3d2e886d1748971e5e7a347131ece25e`  
		Last Modified: Thu, 25 Mar 2021 22:59:56 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43adc9ee5cd36d3802b07723cc589aff1e3db037e675fe58efce4d5462eae66a`  
		Last Modified: Thu, 25 Mar 2021 22:59:58 GMT  
		Size: 11.3 MB (11272061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8e0f63a490f82b0ef607c88accccf9cc79a2d7d215aa19a0f3f49ccd648bfb`  
		Last Modified: Thu, 25 Mar 2021 22:59:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
