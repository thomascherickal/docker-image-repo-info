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
-	[`caddy:2.4.5`](#caddy245)
-	[`caddy:2.4.5-alpine`](#caddy245-alpine)
-	[`caddy:2.4.5-builder`](#caddy245-builder)
-	[`caddy:2.4.5-builder-alpine`](#caddy245-builder-alpine)
-	[`caddy:2.4.5-builder-windowsservercore-1809`](#caddy245-builder-windowsservercore-1809)
-	[`caddy:2.4.5-builder-windowsservercore-ltsc2016`](#caddy245-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.5-windowsservercore`](#caddy245-windowsservercore)
-	[`caddy:2.4.5-windowsservercore-1809`](#caddy245-windowsservercore-1809)
-	[`caddy:2.4.5-windowsservercore-ltsc2016`](#caddy245-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:ddc74d3970803736bb84cbe702d52b7800d14f54d6c0e63c2e70fdedfda05277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:845a00bcc86f8ef55e3ffad434315ea3db858efb04682b6d0881606fb68de9f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14737526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a821fafa344e09dc30d1150bb619f0522186943dfbfe5d01634635c4e11c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:19:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:19:31 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:19:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:19:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:37 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d9d63a262eb117d9f55cf667904b985eb6dd9830783f17146a17a107a7ee19`  
		Last Modified: Tue, 07 Sep 2021 19:20:03 GMT  
		Size: 301.0 KB (301044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d54a459a500730b7153882903986d92e877f472e9d6ead142fab9dcb6464e1`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7c08047a89fabece2d8f1e12d68e1df255fe9c35b5975ff7a707d699359dcf`  
		Last Modified: Tue, 07 Sep 2021 19:20:06 GMT  
		Size: 11.6 MB (11616053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480638d00096415d2de6729bbcc01c75ee3ffeae1dad128c0fb0287c44185632`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:20f1145a9b70aabfa9586f75523258a4a98774618a9625cf02dc2e9c139cfd1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13952683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ef219652d94015e6f435f1d1f504736e9f4b0a0e79b1a4d532d6d18fe5fad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:49:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:49:35 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:49:41 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:49:42 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:49:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:49:48 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254033e1bbf10f9a1641b6005ee6ae290bdec377e00d2e5290e33dc0eb8f9b6`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 301.2 KB (301188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038de9754eec9aa2df09a34c0d7029c335199166de56398d21fb595fd289dd`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a15167bbb466deb6092c935cebbd9a53f872b614c83873105d590b6eb49f0ac`  
		Last Modified: Tue, 07 Sep 2021 19:51:24 GMT  
		Size: 11.0 MB (11018064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35905ee7a334ccab1c6c823badcecdd44820eb72bf4598a513885c773c44b5b`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9dfeb79eec5a0670d371d0441bb86262c154c1bc0b1b60a045698896b6dc59ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13736572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34125796b97ec78f63b7751f271503501af02ec6d00a32966d1099d71fe453e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:57:36 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:57:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:57:39 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:57:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:57:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:57:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:57:46 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:57:47 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:57:52 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:57:52 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:57:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c39987cd6455919d7455feed9aba93a44659ef658fbef5d4d52500beddac5`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 300.4 KB (300356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e223cb6b0d911c9cc6575c496bc4f96f1968db869a8a07694f3f49897920f264`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e52153d20928d86c87f7b2b39f8580cc7323e1b8a59a70936dc2aedc241489`  
		Last Modified: Tue, 07 Sep 2021 19:59:20 GMT  
		Size: 11.0 MB (10999817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231751a6396075ec359101a350a68fd144ab08e31360f7d72c1c7562f931c360`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:758247b074c2f087ee69d246b8765fb5675b6cd56a3c3ef1a5e7ce835a367e22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13654366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b4c65944934a92f9b7c40fbad35a46c8f07383af3795cada31a37f0107fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:39:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:39:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:39:28 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:39:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:39:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:39:33 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:39:34 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:39:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ceb5c04e8fd1a803328fe646ade037fd80af5d1744f9ceda93b4230e5a65b1`  
		Last Modified: Tue, 07 Sep 2021 19:40:18 GMT  
		Size: 301.2 KB (301219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ccdeb47ad54cf62b8f4b6d50208be6d2fe93d863c98e5882a78aeb226fdf1d`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f833026ad56d988c927a40940840f6a33639da2da692c23fb6d794979d6ab8a7`  
		Last Modified: Tue, 07 Sep 2021 19:40:20 GMT  
		Size: 10.6 MB (10635335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e54e7d8eca4b8cf577225887b306d095c98a1636588821fa87515405f3a7e13`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:09f31d1398820362f71bd863c8435a37aaedda9d02fe76c71ccc1c6bc62e46cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13319309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffdd09752fbe7b156120e1250d5383a3670292ae5e9a0e317883f52e732cde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:16:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:16:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:17:07 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:17:56 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:18:01 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:18:05 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:18:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:18:55 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:12 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:21 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d32e3566fcaa11540498ebdd9ecc55cd2e2dca73a6b62317657a9e75749272`  
		Last Modified: Tue, 07 Sep 2021 19:21:13 GMT  
		Size: 303.2 KB (303162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a831abca68890cbd7a89171bb93c9af5c1b102852f0f1f3326ff7c104ced90`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475efcd27e409cc064d659d255fbfb70896b95c3c36149b9a5b8d1abe86e656b`  
		Last Modified: Tue, 07 Sep 2021 19:21:14 GMT  
		Size: 10.2 MB (10197877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a9218ca8c9a1a05649cc5d0eb91f1b2985152d796a63f525c75f5380288bf8`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:d08cf598992165b333bcdea3ad215e6db5f01014f7facd1052d30674b6adbeee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14122948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d162c8bd11aec83d5d81279ca9393020c704e9629f7270c5a36067742b87caf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:41:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:41:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:41:33 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:41:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:41:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:41:49 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:41:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9c7d5d2c4319fc2386cc1a009e57751b8d7a7d807ae0e867e4d6273e06731d`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 301.5 KB (301462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c7b669e195c7cce7cf6d957130645125c1171c464622ceaa01378d18f24e37`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c91b4718f6b0100a4d5f31ab39aa7f732cb3e6d23f084e38e4918a85123a7`  
		Last Modified: Tue, 07 Sep 2021 19:42:45 GMT  
		Size: 11.2 MB (11212039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47704db6d31d2185044e1f3118b87fb2db0caa91fee7ef1cec3ec4a130ad9c`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:6f3b5ea2bfc0b28617452cd422177cc1bf67bd75dc1705cb863fd57d0b43faac
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
$ docker pull caddy@sha256:845a00bcc86f8ef55e3ffad434315ea3db858efb04682b6d0881606fb68de9f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14737526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a821fafa344e09dc30d1150bb619f0522186943dfbfe5d01634635c4e11c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:19:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:19:31 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:19:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:19:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:37 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d9d63a262eb117d9f55cf667904b985eb6dd9830783f17146a17a107a7ee19`  
		Last Modified: Tue, 07 Sep 2021 19:20:03 GMT  
		Size: 301.0 KB (301044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d54a459a500730b7153882903986d92e877f472e9d6ead142fab9dcb6464e1`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7c08047a89fabece2d8f1e12d68e1df255fe9c35b5975ff7a707d699359dcf`  
		Last Modified: Tue, 07 Sep 2021 19:20:06 GMT  
		Size: 11.6 MB (11616053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480638d00096415d2de6729bbcc01c75ee3ffeae1dad128c0fb0287c44185632`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:20f1145a9b70aabfa9586f75523258a4a98774618a9625cf02dc2e9c139cfd1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13952683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ef219652d94015e6f435f1d1f504736e9f4b0a0e79b1a4d532d6d18fe5fad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:49:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:49:35 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:49:41 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:49:42 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:49:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:49:48 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254033e1bbf10f9a1641b6005ee6ae290bdec377e00d2e5290e33dc0eb8f9b6`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 301.2 KB (301188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038de9754eec9aa2df09a34c0d7029c335199166de56398d21fb595fd289dd`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a15167bbb466deb6092c935cebbd9a53f872b614c83873105d590b6eb49f0ac`  
		Last Modified: Tue, 07 Sep 2021 19:51:24 GMT  
		Size: 11.0 MB (11018064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35905ee7a334ccab1c6c823badcecdd44820eb72bf4598a513885c773c44b5b`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9dfeb79eec5a0670d371d0441bb86262c154c1bc0b1b60a045698896b6dc59ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13736572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34125796b97ec78f63b7751f271503501af02ec6d00a32966d1099d71fe453e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:57:36 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:57:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:57:39 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:57:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:57:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:57:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:57:46 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:57:47 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:57:52 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:57:52 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:57:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c39987cd6455919d7455feed9aba93a44659ef658fbef5d4d52500beddac5`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 300.4 KB (300356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e223cb6b0d911c9cc6575c496bc4f96f1968db869a8a07694f3f49897920f264`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e52153d20928d86c87f7b2b39f8580cc7323e1b8a59a70936dc2aedc241489`  
		Last Modified: Tue, 07 Sep 2021 19:59:20 GMT  
		Size: 11.0 MB (10999817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231751a6396075ec359101a350a68fd144ab08e31360f7d72c1c7562f931c360`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:758247b074c2f087ee69d246b8765fb5675b6cd56a3c3ef1a5e7ce835a367e22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13654366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b4c65944934a92f9b7c40fbad35a46c8f07383af3795cada31a37f0107fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:39:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:39:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:39:28 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:39:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:39:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:39:33 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:39:34 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:39:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ceb5c04e8fd1a803328fe646ade037fd80af5d1744f9ceda93b4230e5a65b1`  
		Last Modified: Tue, 07 Sep 2021 19:40:18 GMT  
		Size: 301.2 KB (301219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ccdeb47ad54cf62b8f4b6d50208be6d2fe93d863c98e5882a78aeb226fdf1d`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f833026ad56d988c927a40940840f6a33639da2da692c23fb6d794979d6ab8a7`  
		Last Modified: Tue, 07 Sep 2021 19:40:20 GMT  
		Size: 10.6 MB (10635335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e54e7d8eca4b8cf577225887b306d095c98a1636588821fa87515405f3a7e13`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:09f31d1398820362f71bd863c8435a37aaedda9d02fe76c71ccc1c6bc62e46cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13319309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffdd09752fbe7b156120e1250d5383a3670292ae5e9a0e317883f52e732cde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:16:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:16:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:17:07 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:17:56 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:18:01 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:18:05 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:18:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:18:55 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:12 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:21 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d32e3566fcaa11540498ebdd9ecc55cd2e2dca73a6b62317657a9e75749272`  
		Last Modified: Tue, 07 Sep 2021 19:21:13 GMT  
		Size: 303.2 KB (303162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a831abca68890cbd7a89171bb93c9af5c1b102852f0f1f3326ff7c104ced90`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475efcd27e409cc064d659d255fbfb70896b95c3c36149b9a5b8d1abe86e656b`  
		Last Modified: Tue, 07 Sep 2021 19:21:14 GMT  
		Size: 10.2 MB (10197877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a9218ca8c9a1a05649cc5d0eb91f1b2985152d796a63f525c75f5380288bf8`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d08cf598992165b333bcdea3ad215e6db5f01014f7facd1052d30674b6adbeee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14122948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d162c8bd11aec83d5d81279ca9393020c704e9629f7270c5a36067742b87caf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:41:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:41:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:41:33 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:41:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:41:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:41:49 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:41:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9c7d5d2c4319fc2386cc1a009e57751b8d7a7d807ae0e867e4d6273e06731d`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 301.5 KB (301462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c7b669e195c7cce7cf6d957130645125c1171c464622ceaa01378d18f24e37`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c91b4718f6b0100a4d5f31ab39aa7f732cb3e6d23f084e38e4918a85123a7`  
		Last Modified: Tue, 07 Sep 2021 19:42:45 GMT  
		Size: 11.2 MB (11212039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47704db6d31d2185044e1f3118b87fb2db0caa91fee7ef1cec3ec4a130ad9c`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:9c67813f5545c47b508f871e591fde6f07c649663e1f6444a39a3f78ef5edfdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:7c4854796d5ff77f514c04627f2ec1c375fada1285680273ecf06a2bc8d60cc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121056544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d72fd43a1d67a590271e3f191decedd8b71020ec56d47bb3f2fccd77f452e5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:05 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:21:07 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:22:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:22:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:22:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:22:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:22:59 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:50:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:50:58 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:50:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:50:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:51:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adcdaf11c89113a810db23d523e549d634d7de695a72b0ce98a1f912101262`  
		Last Modified: Mon, 30 Aug 2021 22:01:00 GMT  
		Size: 281.5 KB (281508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b176561691ea11cfe541f3ee363a3aa67e3649eb3273bea62ebeea713eaecd`  
		Last Modified: Mon, 30 Aug 2021 22:00:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a181aec76ea0e8e1b9ceb94467d41cab2fc9417199f12fa6fec3c50137b2933`  
		Last Modified: Thu, 09 Sep 2021 21:32:18 GMT  
		Size: 110.1 MB (110088128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e85de490b301eaafbd51e519e1bf78ed069f65b9f1735b697d139b5f62beaa`  
		Last Modified: Thu, 09 Sep 2021 21:32:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820fbf8070d3ce8dd2131897643ef5f114f3b6460df18bb30178ad42818d7895`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 6.6 MB (6626789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be64ec0930796519b26c01048a13bb77ee8567b37644a29f234f9ad1ca057c72`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 1.2 MB (1244960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c1a24ed462f4f84d50b399f1ff361c49edab51a614e1c02e171c8b1acbbe28`  
		Last Modified: Thu, 09 Sep 2021 21:51:20 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:df768c7d904cfe5f53a02be80a005731d6e73fe96c9059808dbce1c4525c9ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115536665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589c4f054797050b670d7147b81b9f77d40846a8a955fe45875b36743a901c02`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:49:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:49:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:05:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:08:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:08:48 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:08:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:08:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:08:50 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:41:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:41:50 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:41:50 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb221a547a2f49a13c3bbe14f37b0474b2066cece57c67c2fbc1fb07d89aad51`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2968f26f7f14fe309f1a7a85ad968b81a7daa93c078322a84eb5c4192326828`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9feb2689a1f4585cd8be9f2d9ebef91293de2634fb8656a34a8b6ee2a1fc955`  
		Last Modified: Thu, 09 Sep 2021 21:21:18 GMT  
		Size: 105.0 MB (104963985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c005db8fb9ff36fc9e0ce4e66886cafebecd5b7bcc46c08be65094c86e79eb`  
		Last Modified: Thu, 09 Sep 2021 21:20:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c1e636109657a0bb87f7168403a5f2364d5d4790b5b64702fcb241b841c`  
		Last Modified: Thu, 09 Sep 2021 21:43:00 GMT  
		Size: 6.5 MB (6485282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0dee99740bcf1ff7425650fd30e06d203628e08a23e53e51d4a245eec3c353`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 1.2 MB (1177568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db147b9a90d89a0071478428d882f75926adadb6b51474f7035b47e08b04b8`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:66510e6f5ac60a1293e26109be680f90c098e95f5807eb7dc1adfb5c91296d69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114434759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f52bd0e9b05ba459114822b3fed67dcedb8c5d4b7b2fadca9f8a5a24ecad3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 23:51:38 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 23:51:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 23:51:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:45:53 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:57 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:49:00 GMT
WORKDIR /go
# Fri, 10 Sep 2021 00:56:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 00:56:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 00:56:39 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 00:56:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 00:56:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 00:56:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 00:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417f62ae10851eaf03f096c21f2848fdfe2517baf1faffe0a25f4a1f9853e31`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fcbf7d3458d8a294b9a3c72856e5e7ba1372b93f8fc485abecc73f5a8c9b6`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f578778b0e30a8a96971a61afc3fc6db4d30bfa0492a2e76a7258ba63c9f30`  
		Last Modified: Thu, 09 Sep 2021 23:10:09 GMT  
		Size: 104.8 MB (104761719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93a399a67bd75c73ff72134700994ea60add14a1bd3b0d31c62d6c3ce2e2ace`  
		Last Modified: Thu, 09 Sep 2021 23:08:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfe1c03b027f77471402757e95f6f4f82c0d6cd7c4de526518112a1ba027517`  
		Last Modified: Fri, 10 Sep 2021 00:57:51 GMT  
		Size: 5.8 MB (5784816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f7b85f32126cf499c3ce4a1e59e2ad49a8b0e67dfc6ed519033f9df1ddf86`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 1.2 MB (1176262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d94d2c5711b07a6dec9f1f610397ef3ece1750d10c5f6995909f8a82e542e`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3ff72bf69ed60e7be2460e009e5482d1833613b71d61caa64b2632d1bd476b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115219439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b849c371ea6db9199f462a319cfed5552bcdce64f45ef384fd10dd659f7d5b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:41:35 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:46:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:27 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:48:28 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:38:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:38:57 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:38:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:38:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:38:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f2d53f512ea6320316a88e3c306ab2b3a98fccaeb99b4d3ae53c8bdea9e38`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 281.7 KB (281685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70ebbbe112c904d5fa82be2f7801285d376cdf6feea060292096f84b51c668`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e85633e404a49ac115564fa57298187110e7be113c5ff032acfe07513de0d9`  
		Last Modified: Thu, 09 Sep 2021 22:58:24 GMT  
		Size: 104.3 MB (104339130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fd022f582a715a4b1da40be36778771151446f39826676e5d4077c41236106`  
		Last Modified: Thu, 09 Sep 2021 22:58:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb241419bc9c911368f25f2a0f9f85d775eb785aa022f3fb742dd281f960a`  
		Last Modified: Thu, 09 Sep 2021 23:39:35 GMT  
		Size: 6.7 MB (6737938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5e29c4046768a912b16e10abad3b62e5422fc6016f2d35ecbfdd8467e6859`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 1.1 MB (1148145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6994d1faf2f00e16157a93954775e2721979285cc30b828d3814f6d1b21f7`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:9fb0df244fcc2da512b695f9d54178aa6a3536b6496b3a30ca7f23be7adac64c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114019581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa14b6844e2f03eb076817bf5c21767807433bf03846c474cb0cc74097c28b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 00:28:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 31 Aug 2021 00:29:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 00:29:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:29:06 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:31:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:31:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:32:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:32:21 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:11:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:11:34 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:11:38 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:11:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:11:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:12:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539d90ff594fe73c1a1e31b2230e539a965f33143a3c9fbd89507336ed283c2`  
		Last Modified: Tue, 31 Aug 2021 00:52:27 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a17d0ec6ff5411e524016f0ac7033cf7a0a8935f7a5e299d4d7acaad208b26`  
		Last Modified: Tue, 31 Aug 2021 00:52:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc99db09336e6fa3434452924f7d000b95f900c79247baf141252aff2663f8`  
		Last Modified: Thu, 09 Sep 2021 22:52:11 GMT  
		Size: 102.7 MB (102705568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344c38399c8dde1d0551c54c18215c10585c13293c21399eb6c0f1765384cef`  
		Last Modified: Thu, 09 Sep 2021 22:51:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8224fba31f57c4a32f77d62335f2a90f191b76b0c6377b08df77e013f969b0`  
		Last Modified: Thu, 09 Sep 2021 23:12:54 GMT  
		Size: 7.1 MB (7097364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6fad868bb7f9d2057399b0e63a00ac434718e1ae15b711ebd6538230d5d15`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 1.1 MB (1120011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b390087aaec64b1435a6e47fcb0f6d5404981b9c085cc7777616075f6c7c90c4`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ce00c5fb3b7665385ce09f127bb1e442470e68e937ef6cf248affa8c5a5f2520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118449664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cfc73f626d5d8c2436225d97336f140afebc4991de582e1afd6ef5da98ee5b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:33 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:27:17 GMT
ENV GOLANG_VERSION=1.17.1
# Fri, 10 Sep 2021 00:30:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 10 Sep 2021 00:30:35 GMT
ENV GOPATH=/go
# Fri, 10 Sep 2021 00:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:30:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Sep 2021 00:30:38 GMT
WORKDIR /go
# Fri, 10 Sep 2021 01:05:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 01:05:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 01:05:36 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 01:05:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 01:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 01:05:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 01:05:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316d1588ef06afb0d7a96646bb3a1367bce295885797fd976945ed318a4eb9c`  
		Last Modified: Mon, 30 Aug 2021 21:59:27 GMT  
		Size: 281.9 KB (281927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e156a554eded13f9baa4042fb4d12b879560bebfd8aca837bf0b52669f7932`  
		Last Modified: Mon, 30 Aug 2021 21:59:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340913e3811973f494281a53e452b02a3452b65dff8016bb0281f440d907b995`  
		Last Modified: Fri, 10 Sep 2021 00:45:47 GMT  
		Size: 107.6 MB (107637928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f630dccb8f98b0e0c9749886d57178b35e57cb8190c7aae3fcb274cb0b7300`  
		Last Modified: Fri, 10 Sep 2021 00:45:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5eb1022e0b720923e3bbf90f4c4187b742dbe898fbb320597f7a6f18339d0`  
		Last Modified: Fri, 10 Sep 2021 01:06:27 GMT  
		Size: 6.7 MB (6722122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff9a04fa68552015e363e07480e2576f2c693406d1aec848a8d68661294e371`  
		Last Modified: Fri, 10 Sep 2021 01:06:26 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee0066e89945dcd9b9cd7b7fde76d311e2ba9eb2aea4a979a1127ca0da77e5`  
		Last Modified: Fri, 10 Sep 2021 01:06:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:c05c80918ab2e3bdfecd480a6ffb76a5d784d46521cc4e07d03394923cd00d48
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2858877989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bf83018c7cbfec357c464d16b8dae6a41a26166e275948ad315c0d7393ac2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:09:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:09:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:11:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:11:44 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:13:11 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:17:38 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:21:35 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:21:37 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:18:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:18:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:18:39 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:18:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:19:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:19:47 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d2bb4c99ec6467c6c9f474360867d31d27d22bc5be8432059a33a7c602a8`  
		Last Modified: Wed, 25 Aug 2021 13:38:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c31ebb0e52f79c34d0f70b88124ab4959963315dd2da2ec7117063a82d1392`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1935f777314159e43ee24dde17dba33b985a315578d33ec24796ba0ad27f679c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae930e0413fc2f7343e0b46be3ab58503ac4c137e8e6f83c7341838a22c88f3c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6bfd344bdb877d2969098eeb083c114ac4a7ef914d7dcf8eaef4d16e1e248c`  
		Last Modified: Wed, 25 Aug 2021 13:39:17 GMT  
		Size: 25.5 MB (25479918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edda6fbc32a924622fc427734f8d51447a5451f6af8f19da56ef0a27eb34e1a9`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99710b5a5f6d2c1a706493886815250b483d593751506bb096f01ef1d21fd615`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 341.4 KB (341422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4c182170aae5f94cb419bef973f17cd6202c37309480a38333e932f50d0a2a`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19d8d7117b82ef2ee7903f93b8bb7154303b39a1a414461973cf1fcec6164e`  
		Last Modified: Thu, 09 Sep 2021 21:50:44 GMT  
		Size: 145.4 MB (145374753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3826ee6919e32370009775d7e1ea3ffb058f73171f12850c81cd06d7ec08e`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa574525bddae890bf3ee7af7c9ca44962144f7369a75ca44a0c91499f0c5ea`  
		Last Modified: Thu, 09 Sep 2021 22:21:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c383c2091f6f3c8a5bb5f80daf19a417eb4d16e7388332dd8504b854c5d60d7`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca05589790af5b5a3245cb4020121cd24fa7aafcde294bc74d021e1c801f4a8`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe88d3658808037a2f2df97370e9e616f7f61c0b2c81b6fe7d69b5b7decbfda5`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7131f64e32c3073453abaaf1c693d382238a03215217f0fea25131d65252c179`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.7 MB (1665415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8844153c33fc2697353d907cf2a11433cb7d88e55361995778e61d6dc8131801`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:e56175933e7ea82c7f024a59b0388740749e68a8de287a917f91faa0f5b73ff2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448258804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540f1a97650454d989940241d1e55739837273b1056174b03f9d23e6b3a03fe7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:16:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:16:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:16:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:16:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:18:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:18:14 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:19:10 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:21:49 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:25:42 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:25:43 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:20:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:20:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:20:03 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:21:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:21:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f574487f5e33222a294b80d8246d04988a26a38908346c254fa2647c5a7e028d`  
		Last Modified: Wed, 25 Aug 2021 13:39:45 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1bdad4b79465c250e34a289c1b634c4874290ec1fa9da12f91124ba323cb8`  
		Last Modified: Wed, 25 Aug 2021 13:39:44 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca6c7d62e34b14c38c401eb0e5cd89bf7ec9b271c80606691b154e354576ef`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217b8e5d43bb747a0877294acd5f9e1e22f072cc43f97874b9ecb708b70e7d96`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c80e7cfb2acdd3bfa5d45d3d78106e313290ca31797c9e09c7a33d383b758e`  
		Last Modified: Wed, 25 Aug 2021 13:40:10 GMT  
		Size: 25.4 MB (25442011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100167a51a1a9636523c0c49bf6777c5827b991a8d566c9f5d11aa1484485245`  
		Last Modified: Wed, 25 Aug 2021 13:39:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d512787c5e559f25417897aa90a76bf53bf803d34049a88a99cf226d284e96`  
		Last Modified: Wed, 25 Aug 2021 13:39:41 GMT  
		Size: 344.6 KB (344643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebb07b7d9521bf8d2019c0b625d35b815ef26420762706518f517b771a641ff`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8950c36928df1966dbd4308487add3236428fbc4bbf53c6334594fa1589ac4c1`  
		Last Modified: Thu, 09 Sep 2021 21:51:35 GMT  
		Size: 149.9 MB (149860850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51fdf50a7f76c282904490438b43225081dfe0b7965b17cbcbe5696d0f40496`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.5 KB (1519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09564a8db3d28ef4a452036d545bef45bfd9bba2ea702af06ebad5815acca1f`  
		Last Modified: Thu, 09 Sep 2021 22:22:14 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091b186c7f57f040a7c4753bc8b87fdb6c77efe558e44239c050feee6b9a994`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fe2e91a54a2f85d7d88502f47f82c0e7dc6ed3786c9e406b9577207413fdc8`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec7213f2701e2b985f6fd1d12d730aba1ca4c77ae444884b6cabc92c55d8604`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0424b377d7e54c2cf425c9ff6f65e74346d1a33383bd92568bead966ac9b89b4`  
		Last Modified: Thu, 09 Sep 2021 22:22:12 GMT  
		Size: 1.6 MB (1626867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a855cf3d4c553cd4a2241648b20fd2bbb28ce2ac481f3f20d2282aa35dbcb36`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:dd81a9e615feaf5220bab8835282970fecfb2515870f1b63d3540d149855d060
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
$ docker pull caddy@sha256:7c4854796d5ff77f514c04627f2ec1c375fada1285680273ecf06a2bc8d60cc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121056544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d72fd43a1d67a590271e3f191decedd8b71020ec56d47bb3f2fccd77f452e5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:05 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:21:07 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:22:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:22:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:22:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:22:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:22:59 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:50:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:50:58 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:50:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:50:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:51:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adcdaf11c89113a810db23d523e549d634d7de695a72b0ce98a1f912101262`  
		Last Modified: Mon, 30 Aug 2021 22:01:00 GMT  
		Size: 281.5 KB (281508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b176561691ea11cfe541f3ee363a3aa67e3649eb3273bea62ebeea713eaecd`  
		Last Modified: Mon, 30 Aug 2021 22:00:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a181aec76ea0e8e1b9ceb94467d41cab2fc9417199f12fa6fec3c50137b2933`  
		Last Modified: Thu, 09 Sep 2021 21:32:18 GMT  
		Size: 110.1 MB (110088128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e85de490b301eaafbd51e519e1bf78ed069f65b9f1735b697d139b5f62beaa`  
		Last Modified: Thu, 09 Sep 2021 21:32:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820fbf8070d3ce8dd2131897643ef5f114f3b6460df18bb30178ad42818d7895`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 6.6 MB (6626789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be64ec0930796519b26c01048a13bb77ee8567b37644a29f234f9ad1ca057c72`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 1.2 MB (1244960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c1a24ed462f4f84d50b399f1ff361c49edab51a614e1c02e171c8b1acbbe28`  
		Last Modified: Thu, 09 Sep 2021 21:51:20 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:df768c7d904cfe5f53a02be80a005731d6e73fe96c9059808dbce1c4525c9ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115536665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589c4f054797050b670d7147b81b9f77d40846a8a955fe45875b36743a901c02`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:49:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:49:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:05:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:08:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:08:48 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:08:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:08:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:08:50 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:41:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:41:50 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:41:50 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb221a547a2f49a13c3bbe14f37b0474b2066cece57c67c2fbc1fb07d89aad51`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2968f26f7f14fe309f1a7a85ad968b81a7daa93c078322a84eb5c4192326828`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9feb2689a1f4585cd8be9f2d9ebef91293de2634fb8656a34a8b6ee2a1fc955`  
		Last Modified: Thu, 09 Sep 2021 21:21:18 GMT  
		Size: 105.0 MB (104963985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c005db8fb9ff36fc9e0ce4e66886cafebecd5b7bcc46c08be65094c86e79eb`  
		Last Modified: Thu, 09 Sep 2021 21:20:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c1e636109657a0bb87f7168403a5f2364d5d4790b5b64702fcb241b841c`  
		Last Modified: Thu, 09 Sep 2021 21:43:00 GMT  
		Size: 6.5 MB (6485282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0dee99740bcf1ff7425650fd30e06d203628e08a23e53e51d4a245eec3c353`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 1.2 MB (1177568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db147b9a90d89a0071478428d882f75926adadb6b51474f7035b47e08b04b8`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:66510e6f5ac60a1293e26109be680f90c098e95f5807eb7dc1adfb5c91296d69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114434759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f52bd0e9b05ba459114822b3fed67dcedb8c5d4b7b2fadca9f8a5a24ecad3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 23:51:38 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 23:51:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 23:51:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:45:53 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:57 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:49:00 GMT
WORKDIR /go
# Fri, 10 Sep 2021 00:56:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 00:56:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 00:56:39 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 00:56:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 00:56:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 00:56:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 00:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417f62ae10851eaf03f096c21f2848fdfe2517baf1faffe0a25f4a1f9853e31`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fcbf7d3458d8a294b9a3c72856e5e7ba1372b93f8fc485abecc73f5a8c9b6`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f578778b0e30a8a96971a61afc3fc6db4d30bfa0492a2e76a7258ba63c9f30`  
		Last Modified: Thu, 09 Sep 2021 23:10:09 GMT  
		Size: 104.8 MB (104761719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93a399a67bd75c73ff72134700994ea60add14a1bd3b0d31c62d6c3ce2e2ace`  
		Last Modified: Thu, 09 Sep 2021 23:08:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfe1c03b027f77471402757e95f6f4f82c0d6cd7c4de526518112a1ba027517`  
		Last Modified: Fri, 10 Sep 2021 00:57:51 GMT  
		Size: 5.8 MB (5784816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f7b85f32126cf499c3ce4a1e59e2ad49a8b0e67dfc6ed519033f9df1ddf86`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 1.2 MB (1176262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d94d2c5711b07a6dec9f1f610397ef3ece1750d10c5f6995909f8a82e542e`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3ff72bf69ed60e7be2460e009e5482d1833613b71d61caa64b2632d1bd476b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115219439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b849c371ea6db9199f462a319cfed5552bcdce64f45ef384fd10dd659f7d5b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:41:35 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:46:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:27 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:48:28 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:38:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:38:57 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:38:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:38:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:38:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f2d53f512ea6320316a88e3c306ab2b3a98fccaeb99b4d3ae53c8bdea9e38`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 281.7 KB (281685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70ebbbe112c904d5fa82be2f7801285d376cdf6feea060292096f84b51c668`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e85633e404a49ac115564fa57298187110e7be113c5ff032acfe07513de0d9`  
		Last Modified: Thu, 09 Sep 2021 22:58:24 GMT  
		Size: 104.3 MB (104339130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fd022f582a715a4b1da40be36778771151446f39826676e5d4077c41236106`  
		Last Modified: Thu, 09 Sep 2021 22:58:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb241419bc9c911368f25f2a0f9f85d775eb785aa022f3fb742dd281f960a`  
		Last Modified: Thu, 09 Sep 2021 23:39:35 GMT  
		Size: 6.7 MB (6737938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5e29c4046768a912b16e10abad3b62e5422fc6016f2d35ecbfdd8467e6859`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 1.1 MB (1148145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6994d1faf2f00e16157a93954775e2721979285cc30b828d3814f6d1b21f7`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9fb0df244fcc2da512b695f9d54178aa6a3536b6496b3a30ca7f23be7adac64c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114019581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa14b6844e2f03eb076817bf5c21767807433bf03846c474cb0cc74097c28b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 00:28:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 31 Aug 2021 00:29:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 00:29:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:29:06 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:31:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:31:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:32:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:32:21 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:11:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:11:34 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:11:38 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:11:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:11:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:12:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539d90ff594fe73c1a1e31b2230e539a965f33143a3c9fbd89507336ed283c2`  
		Last Modified: Tue, 31 Aug 2021 00:52:27 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a17d0ec6ff5411e524016f0ac7033cf7a0a8935f7a5e299d4d7acaad208b26`  
		Last Modified: Tue, 31 Aug 2021 00:52:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc99db09336e6fa3434452924f7d000b95f900c79247baf141252aff2663f8`  
		Last Modified: Thu, 09 Sep 2021 22:52:11 GMT  
		Size: 102.7 MB (102705568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344c38399c8dde1d0551c54c18215c10585c13293c21399eb6c0f1765384cef`  
		Last Modified: Thu, 09 Sep 2021 22:51:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8224fba31f57c4a32f77d62335f2a90f191b76b0c6377b08df77e013f969b0`  
		Last Modified: Thu, 09 Sep 2021 23:12:54 GMT  
		Size: 7.1 MB (7097364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6fad868bb7f9d2057399b0e63a00ac434718e1ae15b711ebd6538230d5d15`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 1.1 MB (1120011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b390087aaec64b1435a6e47fcb0f6d5404981b9c085cc7777616075f6c7c90c4`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ce00c5fb3b7665385ce09f127bb1e442470e68e937ef6cf248affa8c5a5f2520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118449664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cfc73f626d5d8c2436225d97336f140afebc4991de582e1afd6ef5da98ee5b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:33 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:27:17 GMT
ENV GOLANG_VERSION=1.17.1
# Fri, 10 Sep 2021 00:30:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 10 Sep 2021 00:30:35 GMT
ENV GOPATH=/go
# Fri, 10 Sep 2021 00:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:30:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Sep 2021 00:30:38 GMT
WORKDIR /go
# Fri, 10 Sep 2021 01:05:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 01:05:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 01:05:36 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 01:05:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 01:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 01:05:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 01:05:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316d1588ef06afb0d7a96646bb3a1367bce295885797fd976945ed318a4eb9c`  
		Last Modified: Mon, 30 Aug 2021 21:59:27 GMT  
		Size: 281.9 KB (281927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e156a554eded13f9baa4042fb4d12b879560bebfd8aca837bf0b52669f7932`  
		Last Modified: Mon, 30 Aug 2021 21:59:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340913e3811973f494281a53e452b02a3452b65dff8016bb0281f440d907b995`  
		Last Modified: Fri, 10 Sep 2021 00:45:47 GMT  
		Size: 107.6 MB (107637928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f630dccb8f98b0e0c9749886d57178b35e57cb8190c7aae3fcb274cb0b7300`  
		Last Modified: Fri, 10 Sep 2021 00:45:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5eb1022e0b720923e3bbf90f4c4187b742dbe898fbb320597f7a6f18339d0`  
		Last Modified: Fri, 10 Sep 2021 01:06:27 GMT  
		Size: 6.7 MB (6722122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff9a04fa68552015e363e07480e2576f2c693406d1aec848a8d68661294e371`  
		Last Modified: Fri, 10 Sep 2021 01:06:26 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee0066e89945dcd9b9cd7b7fde76d311e2ba9eb2aea4a979a1127ca0da77e5`  
		Last Modified: Fri, 10 Sep 2021 01:06:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:16873cb6ebb87c355077baa9e6da4fb95ee2388105a0d152fdc47ea77e03f719
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:c05c80918ab2e3bdfecd480a6ffb76a5d784d46521cc4e07d03394923cd00d48
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2858877989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bf83018c7cbfec357c464d16b8dae6a41a26166e275948ad315c0d7393ac2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:09:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:09:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:11:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:11:44 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:13:11 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:17:38 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:21:35 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:21:37 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:18:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:18:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:18:39 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:18:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:19:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:19:47 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d2bb4c99ec6467c6c9f474360867d31d27d22bc5be8432059a33a7c602a8`  
		Last Modified: Wed, 25 Aug 2021 13:38:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c31ebb0e52f79c34d0f70b88124ab4959963315dd2da2ec7117063a82d1392`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1935f777314159e43ee24dde17dba33b985a315578d33ec24796ba0ad27f679c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae930e0413fc2f7343e0b46be3ab58503ac4c137e8e6f83c7341838a22c88f3c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6bfd344bdb877d2969098eeb083c114ac4a7ef914d7dcf8eaef4d16e1e248c`  
		Last Modified: Wed, 25 Aug 2021 13:39:17 GMT  
		Size: 25.5 MB (25479918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edda6fbc32a924622fc427734f8d51447a5451f6af8f19da56ef0a27eb34e1a9`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99710b5a5f6d2c1a706493886815250b483d593751506bb096f01ef1d21fd615`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 341.4 KB (341422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4c182170aae5f94cb419bef973f17cd6202c37309480a38333e932f50d0a2a`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19d8d7117b82ef2ee7903f93b8bb7154303b39a1a414461973cf1fcec6164e`  
		Last Modified: Thu, 09 Sep 2021 21:50:44 GMT  
		Size: 145.4 MB (145374753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3826ee6919e32370009775d7e1ea3ffb058f73171f12850c81cd06d7ec08e`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa574525bddae890bf3ee7af7c9ca44962144f7369a75ca44a0c91499f0c5ea`  
		Last Modified: Thu, 09 Sep 2021 22:21:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c383c2091f6f3c8a5bb5f80daf19a417eb4d16e7388332dd8504b854c5d60d7`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca05589790af5b5a3245cb4020121cd24fa7aafcde294bc74d021e1c801f4a8`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe88d3658808037a2f2df97370e9e616f7f61c0b2c81b6fe7d69b5b7decbfda5`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7131f64e32c3073453abaaf1c693d382238a03215217f0fea25131d65252c179`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.7 MB (1665415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8844153c33fc2697353d907cf2a11433cb7d88e55361995778e61d6dc8131801`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:67f3e7cc995fb43dd91938de46517e8a19471dcc9776214d7d1c8737f0474fd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:e56175933e7ea82c7f024a59b0388740749e68a8de287a917f91faa0f5b73ff2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448258804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540f1a97650454d989940241d1e55739837273b1056174b03f9d23e6b3a03fe7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:16:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:16:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:16:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:16:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:18:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:18:14 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:19:10 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:21:49 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:25:42 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:25:43 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:20:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:20:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:20:03 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:21:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:21:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f574487f5e33222a294b80d8246d04988a26a38908346c254fa2647c5a7e028d`  
		Last Modified: Wed, 25 Aug 2021 13:39:45 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1bdad4b79465c250e34a289c1b634c4874290ec1fa9da12f91124ba323cb8`  
		Last Modified: Wed, 25 Aug 2021 13:39:44 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca6c7d62e34b14c38c401eb0e5cd89bf7ec9b271c80606691b154e354576ef`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217b8e5d43bb747a0877294acd5f9e1e22f072cc43f97874b9ecb708b70e7d96`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c80e7cfb2acdd3bfa5d45d3d78106e313290ca31797c9e09c7a33d383b758e`  
		Last Modified: Wed, 25 Aug 2021 13:40:10 GMT  
		Size: 25.4 MB (25442011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100167a51a1a9636523c0c49bf6777c5827b991a8d566c9f5d11aa1484485245`  
		Last Modified: Wed, 25 Aug 2021 13:39:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d512787c5e559f25417897aa90a76bf53bf803d34049a88a99cf226d284e96`  
		Last Modified: Wed, 25 Aug 2021 13:39:41 GMT  
		Size: 344.6 KB (344643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebb07b7d9521bf8d2019c0b625d35b815ef26420762706518f517b771a641ff`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8950c36928df1966dbd4308487add3236428fbc4bbf53c6334594fa1589ac4c1`  
		Last Modified: Thu, 09 Sep 2021 21:51:35 GMT  
		Size: 149.9 MB (149860850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51fdf50a7f76c282904490438b43225081dfe0b7965b17cbcbe5696d0f40496`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.5 KB (1519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09564a8db3d28ef4a452036d545bef45bfd9bba2ea702af06ebad5815acca1f`  
		Last Modified: Thu, 09 Sep 2021 22:22:14 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091b186c7f57f040a7c4753bc8b87fdb6c77efe558e44239c050feee6b9a994`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fe2e91a54a2f85d7d88502f47f82c0e7dc6ed3786c9e406b9577207413fdc8`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec7213f2701e2b985f6fd1d12d730aba1ca4c77ae444884b6cabc92c55d8604`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0424b377d7e54c2cf425c9ff6f65e74346d1a33383bd92568bead966ac9b89b4`  
		Last Modified: Thu, 09 Sep 2021 22:22:12 GMT  
		Size: 1.6 MB (1626867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a855cf3d4c553cd4a2241648b20fd2bbb28ce2ac481f3f20d2282aa35dbcb36`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:c425c63e4e236cbe5bee3492948f73aa85142a1392096f56c9e952f6cfc61364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9ba0b87da005cab3abb5809cf21dc3b12f8fac8e83c43179846866ba77a9883f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:15e5d6e48e5705c59d244d4506d9259c37b03f6ce2a15bed80e02c1e533ad2ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5`

```console
$ docker pull caddy@sha256:ddc74d3970803736bb84cbe702d52b7800d14f54d6c0e63c2e70fdedfda05277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:2.4.5` - linux; amd64

```console
$ docker pull caddy@sha256:845a00bcc86f8ef55e3ffad434315ea3db858efb04682b6d0881606fb68de9f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14737526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a821fafa344e09dc30d1150bb619f0522186943dfbfe5d01634635c4e11c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:19:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:19:31 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:19:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:19:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:37 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d9d63a262eb117d9f55cf667904b985eb6dd9830783f17146a17a107a7ee19`  
		Last Modified: Tue, 07 Sep 2021 19:20:03 GMT  
		Size: 301.0 KB (301044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d54a459a500730b7153882903986d92e877f472e9d6ead142fab9dcb6464e1`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7c08047a89fabece2d8f1e12d68e1df255fe9c35b5975ff7a707d699359dcf`  
		Last Modified: Tue, 07 Sep 2021 19:20:06 GMT  
		Size: 11.6 MB (11616053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480638d00096415d2de6729bbcc01c75ee3ffeae1dad128c0fb0287c44185632`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5` - linux; arm variant v6

```console
$ docker pull caddy@sha256:20f1145a9b70aabfa9586f75523258a4a98774618a9625cf02dc2e9c139cfd1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13952683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ef219652d94015e6f435f1d1f504736e9f4b0a0e79b1a4d532d6d18fe5fad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:49:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:49:35 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:49:41 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:49:42 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:49:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:49:48 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254033e1bbf10f9a1641b6005ee6ae290bdec377e00d2e5290e33dc0eb8f9b6`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 301.2 KB (301188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038de9754eec9aa2df09a34c0d7029c335199166de56398d21fb595fd289dd`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a15167bbb466deb6092c935cebbd9a53f872b614c83873105d590b6eb49f0ac`  
		Last Modified: Tue, 07 Sep 2021 19:51:24 GMT  
		Size: 11.0 MB (11018064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35905ee7a334ccab1c6c823badcecdd44820eb72bf4598a513885c773c44b5b`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9dfeb79eec5a0670d371d0441bb86262c154c1bc0b1b60a045698896b6dc59ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13736572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34125796b97ec78f63b7751f271503501af02ec6d00a32966d1099d71fe453e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:57:36 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:57:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:57:39 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:57:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:57:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:57:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:57:46 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:57:47 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:57:52 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:57:52 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:57:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c39987cd6455919d7455feed9aba93a44659ef658fbef5d4d52500beddac5`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 300.4 KB (300356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e223cb6b0d911c9cc6575c496bc4f96f1968db869a8a07694f3f49897920f264`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e52153d20928d86c87f7b2b39f8580cc7323e1b8a59a70936dc2aedc241489`  
		Last Modified: Tue, 07 Sep 2021 19:59:20 GMT  
		Size: 11.0 MB (10999817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231751a6396075ec359101a350a68fd144ab08e31360f7d72c1c7562f931c360`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:758247b074c2f087ee69d246b8765fb5675b6cd56a3c3ef1a5e7ce835a367e22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13654366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b4c65944934a92f9b7c40fbad35a46c8f07383af3795cada31a37f0107fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:39:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:39:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:39:28 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:39:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:39:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:39:33 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:39:34 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:39:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ceb5c04e8fd1a803328fe646ade037fd80af5d1744f9ceda93b4230e5a65b1`  
		Last Modified: Tue, 07 Sep 2021 19:40:18 GMT  
		Size: 301.2 KB (301219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ccdeb47ad54cf62b8f4b6d50208be6d2fe93d863c98e5882a78aeb226fdf1d`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f833026ad56d988c927a40940840f6a33639da2da692c23fb6d794979d6ab8a7`  
		Last Modified: Tue, 07 Sep 2021 19:40:20 GMT  
		Size: 10.6 MB (10635335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e54e7d8eca4b8cf577225887b306d095c98a1636588821fa87515405f3a7e13`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5` - linux; ppc64le

```console
$ docker pull caddy@sha256:09f31d1398820362f71bd863c8435a37aaedda9d02fe76c71ccc1c6bc62e46cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13319309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffdd09752fbe7b156120e1250d5383a3670292ae5e9a0e317883f52e732cde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:16:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:16:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:17:07 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:17:56 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:18:01 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:18:05 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:18:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:18:55 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:12 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:21 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d32e3566fcaa11540498ebdd9ecc55cd2e2dca73a6b62317657a9e75749272`  
		Last Modified: Tue, 07 Sep 2021 19:21:13 GMT  
		Size: 303.2 KB (303162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a831abca68890cbd7a89171bb93c9af5c1b102852f0f1f3326ff7c104ced90`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475efcd27e409cc064d659d255fbfb70896b95c3c36149b9a5b8d1abe86e656b`  
		Last Modified: Tue, 07 Sep 2021 19:21:14 GMT  
		Size: 10.2 MB (10197877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a9218ca8c9a1a05649cc5d0eb91f1b2985152d796a63f525c75f5380288bf8`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5` - linux; s390x

```console
$ docker pull caddy@sha256:d08cf598992165b333bcdea3ad215e6db5f01014f7facd1052d30674b6adbeee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14122948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d162c8bd11aec83d5d81279ca9393020c704e9629f7270c5a36067742b87caf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:41:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:41:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:41:33 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:41:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:41:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:41:49 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:41:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9c7d5d2c4319fc2386cc1a009e57751b8d7a7d807ae0e867e4d6273e06731d`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 301.5 KB (301462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c7b669e195c7cce7cf6d957130645125c1171c464622ceaa01378d18f24e37`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c91b4718f6b0100a4d5f31ab39aa7f732cb3e6d23f084e38e4918a85123a7`  
		Last Modified: Tue, 07 Sep 2021 19:42:45 GMT  
		Size: 11.2 MB (11212039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47704db6d31d2185044e1f3118b87fb2db0caa91fee7ef1cec3ec4a130ad9c`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-alpine`

```console
$ docker pull caddy@sha256:6f3b5ea2bfc0b28617452cd422177cc1bf67bd75dc1705cb863fd57d0b43faac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.5-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:845a00bcc86f8ef55e3ffad434315ea3db858efb04682b6d0881606fb68de9f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14737526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a821fafa344e09dc30d1150bb619f0522186943dfbfe5d01634635c4e11c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:19:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:19:31 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:19:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:19:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:37 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d9d63a262eb117d9f55cf667904b985eb6dd9830783f17146a17a107a7ee19`  
		Last Modified: Tue, 07 Sep 2021 19:20:03 GMT  
		Size: 301.0 KB (301044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d54a459a500730b7153882903986d92e877f472e9d6ead142fab9dcb6464e1`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7c08047a89fabece2d8f1e12d68e1df255fe9c35b5975ff7a707d699359dcf`  
		Last Modified: Tue, 07 Sep 2021 19:20:06 GMT  
		Size: 11.6 MB (11616053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480638d00096415d2de6729bbcc01c75ee3ffeae1dad128c0fb0287c44185632`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:20f1145a9b70aabfa9586f75523258a4a98774618a9625cf02dc2e9c139cfd1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13952683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ef219652d94015e6f435f1d1f504736e9f4b0a0e79b1a4d532d6d18fe5fad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:49:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:49:35 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:49:41 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:49:42 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:49:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:49:48 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254033e1bbf10f9a1641b6005ee6ae290bdec377e00d2e5290e33dc0eb8f9b6`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 301.2 KB (301188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038de9754eec9aa2df09a34c0d7029c335199166de56398d21fb595fd289dd`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a15167bbb466deb6092c935cebbd9a53f872b614c83873105d590b6eb49f0ac`  
		Last Modified: Tue, 07 Sep 2021 19:51:24 GMT  
		Size: 11.0 MB (11018064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35905ee7a334ccab1c6c823badcecdd44820eb72bf4598a513885c773c44b5b`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9dfeb79eec5a0670d371d0441bb86262c154c1bc0b1b60a045698896b6dc59ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13736572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34125796b97ec78f63b7751f271503501af02ec6d00a32966d1099d71fe453e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:57:36 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:57:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:57:39 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:57:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:57:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:57:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:57:46 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:57:47 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:57:52 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:57:52 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:57:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c39987cd6455919d7455feed9aba93a44659ef658fbef5d4d52500beddac5`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 300.4 KB (300356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e223cb6b0d911c9cc6575c496bc4f96f1968db869a8a07694f3f49897920f264`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e52153d20928d86c87f7b2b39f8580cc7323e1b8a59a70936dc2aedc241489`  
		Last Modified: Tue, 07 Sep 2021 19:59:20 GMT  
		Size: 11.0 MB (10999817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231751a6396075ec359101a350a68fd144ab08e31360f7d72c1c7562f931c360`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:758247b074c2f087ee69d246b8765fb5675b6cd56a3c3ef1a5e7ce835a367e22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13654366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b4c65944934a92f9b7c40fbad35a46c8f07383af3795cada31a37f0107fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:39:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:39:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:39:28 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:39:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:39:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:39:33 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:39:34 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:39:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ceb5c04e8fd1a803328fe646ade037fd80af5d1744f9ceda93b4230e5a65b1`  
		Last Modified: Tue, 07 Sep 2021 19:40:18 GMT  
		Size: 301.2 KB (301219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ccdeb47ad54cf62b8f4b6d50208be6d2fe93d863c98e5882a78aeb226fdf1d`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f833026ad56d988c927a40940840f6a33639da2da692c23fb6d794979d6ab8a7`  
		Last Modified: Tue, 07 Sep 2021 19:40:20 GMT  
		Size: 10.6 MB (10635335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e54e7d8eca4b8cf577225887b306d095c98a1636588821fa87515405f3a7e13`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:09f31d1398820362f71bd863c8435a37aaedda9d02fe76c71ccc1c6bc62e46cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13319309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffdd09752fbe7b156120e1250d5383a3670292ae5e9a0e317883f52e732cde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:16:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:16:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:17:07 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:17:56 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:18:01 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:18:05 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:18:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:18:55 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:12 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:21 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d32e3566fcaa11540498ebdd9ecc55cd2e2dca73a6b62317657a9e75749272`  
		Last Modified: Tue, 07 Sep 2021 19:21:13 GMT  
		Size: 303.2 KB (303162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a831abca68890cbd7a89171bb93c9af5c1b102852f0f1f3326ff7c104ced90`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475efcd27e409cc064d659d255fbfb70896b95c3c36149b9a5b8d1abe86e656b`  
		Last Modified: Tue, 07 Sep 2021 19:21:14 GMT  
		Size: 10.2 MB (10197877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a9218ca8c9a1a05649cc5d0eb91f1b2985152d796a63f525c75f5380288bf8`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d08cf598992165b333bcdea3ad215e6db5f01014f7facd1052d30674b6adbeee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14122948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d162c8bd11aec83d5d81279ca9393020c704e9629f7270c5a36067742b87caf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:41:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:41:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:41:33 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:41:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:41:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:41:49 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:41:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9c7d5d2c4319fc2386cc1a009e57751b8d7a7d807ae0e867e4d6273e06731d`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 301.5 KB (301462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c7b669e195c7cce7cf6d957130645125c1171c464622ceaa01378d18f24e37`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c91b4718f6b0100a4d5f31ab39aa7f732cb3e6d23f084e38e4918a85123a7`  
		Last Modified: Tue, 07 Sep 2021 19:42:45 GMT  
		Size: 11.2 MB (11212039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47704db6d31d2185044e1f3118b87fb2db0caa91fee7ef1cec3ec4a130ad9c`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-builder`

```console
$ docker pull caddy@sha256:9c67813f5545c47b508f871e591fde6f07c649663e1f6444a39a3f78ef5edfdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:2.4.5-builder` - linux; amd64

```console
$ docker pull caddy@sha256:7c4854796d5ff77f514c04627f2ec1c375fada1285680273ecf06a2bc8d60cc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121056544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d72fd43a1d67a590271e3f191decedd8b71020ec56d47bb3f2fccd77f452e5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:05 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:21:07 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:22:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:22:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:22:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:22:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:22:59 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:50:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:50:58 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:50:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:50:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:51:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adcdaf11c89113a810db23d523e549d634d7de695a72b0ce98a1f912101262`  
		Last Modified: Mon, 30 Aug 2021 22:01:00 GMT  
		Size: 281.5 KB (281508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b176561691ea11cfe541f3ee363a3aa67e3649eb3273bea62ebeea713eaecd`  
		Last Modified: Mon, 30 Aug 2021 22:00:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a181aec76ea0e8e1b9ceb94467d41cab2fc9417199f12fa6fec3c50137b2933`  
		Last Modified: Thu, 09 Sep 2021 21:32:18 GMT  
		Size: 110.1 MB (110088128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e85de490b301eaafbd51e519e1bf78ed069f65b9f1735b697d139b5f62beaa`  
		Last Modified: Thu, 09 Sep 2021 21:32:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820fbf8070d3ce8dd2131897643ef5f114f3b6460df18bb30178ad42818d7895`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 6.6 MB (6626789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be64ec0930796519b26c01048a13bb77ee8567b37644a29f234f9ad1ca057c72`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 1.2 MB (1244960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c1a24ed462f4f84d50b399f1ff361c49edab51a614e1c02e171c8b1acbbe28`  
		Last Modified: Thu, 09 Sep 2021 21:51:20 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:df768c7d904cfe5f53a02be80a005731d6e73fe96c9059808dbce1c4525c9ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115536665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589c4f054797050b670d7147b81b9f77d40846a8a955fe45875b36743a901c02`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:49:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:49:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:05:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:08:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:08:48 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:08:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:08:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:08:50 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:41:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:41:50 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:41:50 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb221a547a2f49a13c3bbe14f37b0474b2066cece57c67c2fbc1fb07d89aad51`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2968f26f7f14fe309f1a7a85ad968b81a7daa93c078322a84eb5c4192326828`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9feb2689a1f4585cd8be9f2d9ebef91293de2634fb8656a34a8b6ee2a1fc955`  
		Last Modified: Thu, 09 Sep 2021 21:21:18 GMT  
		Size: 105.0 MB (104963985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c005db8fb9ff36fc9e0ce4e66886cafebecd5b7bcc46c08be65094c86e79eb`  
		Last Modified: Thu, 09 Sep 2021 21:20:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c1e636109657a0bb87f7168403a5f2364d5d4790b5b64702fcb241b841c`  
		Last Modified: Thu, 09 Sep 2021 21:43:00 GMT  
		Size: 6.5 MB (6485282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0dee99740bcf1ff7425650fd30e06d203628e08a23e53e51d4a245eec3c353`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 1.2 MB (1177568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db147b9a90d89a0071478428d882f75926adadb6b51474f7035b47e08b04b8`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:66510e6f5ac60a1293e26109be680f90c098e95f5807eb7dc1adfb5c91296d69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114434759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f52bd0e9b05ba459114822b3fed67dcedb8c5d4b7b2fadca9f8a5a24ecad3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 23:51:38 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 23:51:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 23:51:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:45:53 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:57 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:49:00 GMT
WORKDIR /go
# Fri, 10 Sep 2021 00:56:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 00:56:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 00:56:39 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 00:56:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 00:56:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 00:56:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 00:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417f62ae10851eaf03f096c21f2848fdfe2517baf1faffe0a25f4a1f9853e31`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fcbf7d3458d8a294b9a3c72856e5e7ba1372b93f8fc485abecc73f5a8c9b6`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f578778b0e30a8a96971a61afc3fc6db4d30bfa0492a2e76a7258ba63c9f30`  
		Last Modified: Thu, 09 Sep 2021 23:10:09 GMT  
		Size: 104.8 MB (104761719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93a399a67bd75c73ff72134700994ea60add14a1bd3b0d31c62d6c3ce2e2ace`  
		Last Modified: Thu, 09 Sep 2021 23:08:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfe1c03b027f77471402757e95f6f4f82c0d6cd7c4de526518112a1ba027517`  
		Last Modified: Fri, 10 Sep 2021 00:57:51 GMT  
		Size: 5.8 MB (5784816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f7b85f32126cf499c3ce4a1e59e2ad49a8b0e67dfc6ed519033f9df1ddf86`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 1.2 MB (1176262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d94d2c5711b07a6dec9f1f610397ef3ece1750d10c5f6995909f8a82e542e`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3ff72bf69ed60e7be2460e009e5482d1833613b71d61caa64b2632d1bd476b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115219439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b849c371ea6db9199f462a319cfed5552bcdce64f45ef384fd10dd659f7d5b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:41:35 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:46:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:27 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:48:28 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:38:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:38:57 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:38:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:38:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:38:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f2d53f512ea6320316a88e3c306ab2b3a98fccaeb99b4d3ae53c8bdea9e38`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 281.7 KB (281685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70ebbbe112c904d5fa82be2f7801285d376cdf6feea060292096f84b51c668`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e85633e404a49ac115564fa57298187110e7be113c5ff032acfe07513de0d9`  
		Last Modified: Thu, 09 Sep 2021 22:58:24 GMT  
		Size: 104.3 MB (104339130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fd022f582a715a4b1da40be36778771151446f39826676e5d4077c41236106`  
		Last Modified: Thu, 09 Sep 2021 22:58:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb241419bc9c911368f25f2a0f9f85d775eb785aa022f3fb742dd281f960a`  
		Last Modified: Thu, 09 Sep 2021 23:39:35 GMT  
		Size: 6.7 MB (6737938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5e29c4046768a912b16e10abad3b62e5422fc6016f2d35ecbfdd8467e6859`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 1.1 MB (1148145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6994d1faf2f00e16157a93954775e2721979285cc30b828d3814f6d1b21f7`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:9fb0df244fcc2da512b695f9d54178aa6a3536b6496b3a30ca7f23be7adac64c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114019581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa14b6844e2f03eb076817bf5c21767807433bf03846c474cb0cc74097c28b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 00:28:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 31 Aug 2021 00:29:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 00:29:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:29:06 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:31:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:31:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:32:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:32:21 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:11:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:11:34 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:11:38 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:11:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:11:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:12:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539d90ff594fe73c1a1e31b2230e539a965f33143a3c9fbd89507336ed283c2`  
		Last Modified: Tue, 31 Aug 2021 00:52:27 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a17d0ec6ff5411e524016f0ac7033cf7a0a8935f7a5e299d4d7acaad208b26`  
		Last Modified: Tue, 31 Aug 2021 00:52:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc99db09336e6fa3434452924f7d000b95f900c79247baf141252aff2663f8`  
		Last Modified: Thu, 09 Sep 2021 22:52:11 GMT  
		Size: 102.7 MB (102705568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344c38399c8dde1d0551c54c18215c10585c13293c21399eb6c0f1765384cef`  
		Last Modified: Thu, 09 Sep 2021 22:51:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8224fba31f57c4a32f77d62335f2a90f191b76b0c6377b08df77e013f969b0`  
		Last Modified: Thu, 09 Sep 2021 23:12:54 GMT  
		Size: 7.1 MB (7097364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6fad868bb7f9d2057399b0e63a00ac434718e1ae15b711ebd6538230d5d15`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 1.1 MB (1120011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b390087aaec64b1435a6e47fcb0f6d5404981b9c085cc7777616075f6c7c90c4`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder` - linux; s390x

```console
$ docker pull caddy@sha256:ce00c5fb3b7665385ce09f127bb1e442470e68e937ef6cf248affa8c5a5f2520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118449664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cfc73f626d5d8c2436225d97336f140afebc4991de582e1afd6ef5da98ee5b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:33 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:27:17 GMT
ENV GOLANG_VERSION=1.17.1
# Fri, 10 Sep 2021 00:30:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 10 Sep 2021 00:30:35 GMT
ENV GOPATH=/go
# Fri, 10 Sep 2021 00:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:30:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Sep 2021 00:30:38 GMT
WORKDIR /go
# Fri, 10 Sep 2021 01:05:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 01:05:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 01:05:36 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 01:05:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 01:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 01:05:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 01:05:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316d1588ef06afb0d7a96646bb3a1367bce295885797fd976945ed318a4eb9c`  
		Last Modified: Mon, 30 Aug 2021 21:59:27 GMT  
		Size: 281.9 KB (281927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e156a554eded13f9baa4042fb4d12b879560bebfd8aca837bf0b52669f7932`  
		Last Modified: Mon, 30 Aug 2021 21:59:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340913e3811973f494281a53e452b02a3452b65dff8016bb0281f440d907b995`  
		Last Modified: Fri, 10 Sep 2021 00:45:47 GMT  
		Size: 107.6 MB (107637928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f630dccb8f98b0e0c9749886d57178b35e57cb8190c7aae3fcb274cb0b7300`  
		Last Modified: Fri, 10 Sep 2021 00:45:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5eb1022e0b720923e3bbf90f4c4187b742dbe898fbb320597f7a6f18339d0`  
		Last Modified: Fri, 10 Sep 2021 01:06:27 GMT  
		Size: 6.7 MB (6722122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff9a04fa68552015e363e07480e2576f2c693406d1aec848a8d68661294e371`  
		Last Modified: Fri, 10 Sep 2021 01:06:26 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee0066e89945dcd9b9cd7b7fde76d311e2ba9eb2aea4a979a1127ca0da77e5`  
		Last Modified: Fri, 10 Sep 2021 01:06:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:c05c80918ab2e3bdfecd480a6ffb76a5d784d46521cc4e07d03394923cd00d48
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2858877989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bf83018c7cbfec357c464d16b8dae6a41a26166e275948ad315c0d7393ac2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:09:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:09:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:11:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:11:44 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:13:11 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:17:38 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:21:35 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:21:37 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:18:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:18:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:18:39 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:18:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:19:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:19:47 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d2bb4c99ec6467c6c9f474360867d31d27d22bc5be8432059a33a7c602a8`  
		Last Modified: Wed, 25 Aug 2021 13:38:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c31ebb0e52f79c34d0f70b88124ab4959963315dd2da2ec7117063a82d1392`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1935f777314159e43ee24dde17dba33b985a315578d33ec24796ba0ad27f679c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae930e0413fc2f7343e0b46be3ab58503ac4c137e8e6f83c7341838a22c88f3c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6bfd344bdb877d2969098eeb083c114ac4a7ef914d7dcf8eaef4d16e1e248c`  
		Last Modified: Wed, 25 Aug 2021 13:39:17 GMT  
		Size: 25.5 MB (25479918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edda6fbc32a924622fc427734f8d51447a5451f6af8f19da56ef0a27eb34e1a9`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99710b5a5f6d2c1a706493886815250b483d593751506bb096f01ef1d21fd615`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 341.4 KB (341422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4c182170aae5f94cb419bef973f17cd6202c37309480a38333e932f50d0a2a`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19d8d7117b82ef2ee7903f93b8bb7154303b39a1a414461973cf1fcec6164e`  
		Last Modified: Thu, 09 Sep 2021 21:50:44 GMT  
		Size: 145.4 MB (145374753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3826ee6919e32370009775d7e1ea3ffb058f73171f12850c81cd06d7ec08e`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa574525bddae890bf3ee7af7c9ca44962144f7369a75ca44a0c91499f0c5ea`  
		Last Modified: Thu, 09 Sep 2021 22:21:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c383c2091f6f3c8a5bb5f80daf19a417eb4d16e7388332dd8504b854c5d60d7`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca05589790af5b5a3245cb4020121cd24fa7aafcde294bc74d021e1c801f4a8`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe88d3658808037a2f2df97370e9e616f7f61c0b2c81b6fe7d69b5b7decbfda5`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7131f64e32c3073453abaaf1c693d382238a03215217f0fea25131d65252c179`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.7 MB (1665415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8844153c33fc2697353d907cf2a11433cb7d88e55361995778e61d6dc8131801`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:e56175933e7ea82c7f024a59b0388740749e68a8de287a917f91faa0f5b73ff2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448258804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540f1a97650454d989940241d1e55739837273b1056174b03f9d23e6b3a03fe7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:16:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:16:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:16:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:16:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:18:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:18:14 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:19:10 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:21:49 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:25:42 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:25:43 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:20:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:20:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:20:03 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:21:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:21:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f574487f5e33222a294b80d8246d04988a26a38908346c254fa2647c5a7e028d`  
		Last Modified: Wed, 25 Aug 2021 13:39:45 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1bdad4b79465c250e34a289c1b634c4874290ec1fa9da12f91124ba323cb8`  
		Last Modified: Wed, 25 Aug 2021 13:39:44 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca6c7d62e34b14c38c401eb0e5cd89bf7ec9b271c80606691b154e354576ef`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217b8e5d43bb747a0877294acd5f9e1e22f072cc43f97874b9ecb708b70e7d96`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c80e7cfb2acdd3bfa5d45d3d78106e313290ca31797c9e09c7a33d383b758e`  
		Last Modified: Wed, 25 Aug 2021 13:40:10 GMT  
		Size: 25.4 MB (25442011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100167a51a1a9636523c0c49bf6777c5827b991a8d566c9f5d11aa1484485245`  
		Last Modified: Wed, 25 Aug 2021 13:39:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d512787c5e559f25417897aa90a76bf53bf803d34049a88a99cf226d284e96`  
		Last Modified: Wed, 25 Aug 2021 13:39:41 GMT  
		Size: 344.6 KB (344643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebb07b7d9521bf8d2019c0b625d35b815ef26420762706518f517b771a641ff`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8950c36928df1966dbd4308487add3236428fbc4bbf53c6334594fa1589ac4c1`  
		Last Modified: Thu, 09 Sep 2021 21:51:35 GMT  
		Size: 149.9 MB (149860850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51fdf50a7f76c282904490438b43225081dfe0b7965b17cbcbe5696d0f40496`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.5 KB (1519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09564a8db3d28ef4a452036d545bef45bfd9bba2ea702af06ebad5815acca1f`  
		Last Modified: Thu, 09 Sep 2021 22:22:14 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091b186c7f57f040a7c4753bc8b87fdb6c77efe558e44239c050feee6b9a994`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fe2e91a54a2f85d7d88502f47f82c0e7dc6ed3786c9e406b9577207413fdc8`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec7213f2701e2b985f6fd1d12d730aba1ca4c77ae444884b6cabc92c55d8604`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0424b377d7e54c2cf425c9ff6f65e74346d1a33383bd92568bead966ac9b89b4`  
		Last Modified: Thu, 09 Sep 2021 22:22:12 GMT  
		Size: 1.6 MB (1626867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a855cf3d4c553cd4a2241648b20fd2bbb28ce2ac481f3f20d2282aa35dbcb36`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-builder-alpine`

```console
$ docker pull caddy@sha256:dd81a9e615feaf5220bab8835282970fecfb2515870f1b63d3540d149855d060
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.5-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:7c4854796d5ff77f514c04627f2ec1c375fada1285680273ecf06a2bc8d60cc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121056544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d72fd43a1d67a590271e3f191decedd8b71020ec56d47bb3f2fccd77f452e5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:05 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:21:07 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:22:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:22:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:22:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:22:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:22:59 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:50:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:50:58 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:50:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:50:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:51:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adcdaf11c89113a810db23d523e549d634d7de695a72b0ce98a1f912101262`  
		Last Modified: Mon, 30 Aug 2021 22:01:00 GMT  
		Size: 281.5 KB (281508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b176561691ea11cfe541f3ee363a3aa67e3649eb3273bea62ebeea713eaecd`  
		Last Modified: Mon, 30 Aug 2021 22:00:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a181aec76ea0e8e1b9ceb94467d41cab2fc9417199f12fa6fec3c50137b2933`  
		Last Modified: Thu, 09 Sep 2021 21:32:18 GMT  
		Size: 110.1 MB (110088128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e85de490b301eaafbd51e519e1bf78ed069f65b9f1735b697d139b5f62beaa`  
		Last Modified: Thu, 09 Sep 2021 21:32:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820fbf8070d3ce8dd2131897643ef5f114f3b6460df18bb30178ad42818d7895`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 6.6 MB (6626789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be64ec0930796519b26c01048a13bb77ee8567b37644a29f234f9ad1ca057c72`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 1.2 MB (1244960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c1a24ed462f4f84d50b399f1ff361c49edab51a614e1c02e171c8b1acbbe28`  
		Last Modified: Thu, 09 Sep 2021 21:51:20 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:df768c7d904cfe5f53a02be80a005731d6e73fe96c9059808dbce1c4525c9ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115536665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589c4f054797050b670d7147b81b9f77d40846a8a955fe45875b36743a901c02`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:49:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:49:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:05:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:08:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:08:48 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:08:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:08:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:08:50 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:41:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:41:50 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:41:50 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb221a547a2f49a13c3bbe14f37b0474b2066cece57c67c2fbc1fb07d89aad51`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2968f26f7f14fe309f1a7a85ad968b81a7daa93c078322a84eb5c4192326828`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9feb2689a1f4585cd8be9f2d9ebef91293de2634fb8656a34a8b6ee2a1fc955`  
		Last Modified: Thu, 09 Sep 2021 21:21:18 GMT  
		Size: 105.0 MB (104963985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c005db8fb9ff36fc9e0ce4e66886cafebecd5b7bcc46c08be65094c86e79eb`  
		Last Modified: Thu, 09 Sep 2021 21:20:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c1e636109657a0bb87f7168403a5f2364d5d4790b5b64702fcb241b841c`  
		Last Modified: Thu, 09 Sep 2021 21:43:00 GMT  
		Size: 6.5 MB (6485282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0dee99740bcf1ff7425650fd30e06d203628e08a23e53e51d4a245eec3c353`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 1.2 MB (1177568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db147b9a90d89a0071478428d882f75926adadb6b51474f7035b47e08b04b8`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:66510e6f5ac60a1293e26109be680f90c098e95f5807eb7dc1adfb5c91296d69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114434759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f52bd0e9b05ba459114822b3fed67dcedb8c5d4b7b2fadca9f8a5a24ecad3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 23:51:38 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 23:51:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 23:51:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:45:53 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:57 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:49:00 GMT
WORKDIR /go
# Fri, 10 Sep 2021 00:56:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 00:56:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 00:56:39 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 00:56:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 00:56:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 00:56:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 00:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417f62ae10851eaf03f096c21f2848fdfe2517baf1faffe0a25f4a1f9853e31`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fcbf7d3458d8a294b9a3c72856e5e7ba1372b93f8fc485abecc73f5a8c9b6`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f578778b0e30a8a96971a61afc3fc6db4d30bfa0492a2e76a7258ba63c9f30`  
		Last Modified: Thu, 09 Sep 2021 23:10:09 GMT  
		Size: 104.8 MB (104761719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93a399a67bd75c73ff72134700994ea60add14a1bd3b0d31c62d6c3ce2e2ace`  
		Last Modified: Thu, 09 Sep 2021 23:08:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfe1c03b027f77471402757e95f6f4f82c0d6cd7c4de526518112a1ba027517`  
		Last Modified: Fri, 10 Sep 2021 00:57:51 GMT  
		Size: 5.8 MB (5784816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f7b85f32126cf499c3ce4a1e59e2ad49a8b0e67dfc6ed519033f9df1ddf86`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 1.2 MB (1176262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d94d2c5711b07a6dec9f1f610397ef3ece1750d10c5f6995909f8a82e542e`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3ff72bf69ed60e7be2460e009e5482d1833613b71d61caa64b2632d1bd476b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115219439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b849c371ea6db9199f462a319cfed5552bcdce64f45ef384fd10dd659f7d5b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:41:35 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:46:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:27 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:48:28 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:38:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:38:57 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:38:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:38:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:38:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f2d53f512ea6320316a88e3c306ab2b3a98fccaeb99b4d3ae53c8bdea9e38`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 281.7 KB (281685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70ebbbe112c904d5fa82be2f7801285d376cdf6feea060292096f84b51c668`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e85633e404a49ac115564fa57298187110e7be113c5ff032acfe07513de0d9`  
		Last Modified: Thu, 09 Sep 2021 22:58:24 GMT  
		Size: 104.3 MB (104339130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fd022f582a715a4b1da40be36778771151446f39826676e5d4077c41236106`  
		Last Modified: Thu, 09 Sep 2021 22:58:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb241419bc9c911368f25f2a0f9f85d775eb785aa022f3fb742dd281f960a`  
		Last Modified: Thu, 09 Sep 2021 23:39:35 GMT  
		Size: 6.7 MB (6737938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5e29c4046768a912b16e10abad3b62e5422fc6016f2d35ecbfdd8467e6859`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 1.1 MB (1148145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6994d1faf2f00e16157a93954775e2721979285cc30b828d3814f6d1b21f7`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9fb0df244fcc2da512b695f9d54178aa6a3536b6496b3a30ca7f23be7adac64c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114019581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa14b6844e2f03eb076817bf5c21767807433bf03846c474cb0cc74097c28b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 00:28:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 31 Aug 2021 00:29:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 00:29:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:29:06 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:31:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:31:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:32:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:32:21 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:11:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:11:34 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:11:38 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:11:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:11:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:12:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539d90ff594fe73c1a1e31b2230e539a965f33143a3c9fbd89507336ed283c2`  
		Last Modified: Tue, 31 Aug 2021 00:52:27 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a17d0ec6ff5411e524016f0ac7033cf7a0a8935f7a5e299d4d7acaad208b26`  
		Last Modified: Tue, 31 Aug 2021 00:52:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc99db09336e6fa3434452924f7d000b95f900c79247baf141252aff2663f8`  
		Last Modified: Thu, 09 Sep 2021 22:52:11 GMT  
		Size: 102.7 MB (102705568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344c38399c8dde1d0551c54c18215c10585c13293c21399eb6c0f1765384cef`  
		Last Modified: Thu, 09 Sep 2021 22:51:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8224fba31f57c4a32f77d62335f2a90f191b76b0c6377b08df77e013f969b0`  
		Last Modified: Thu, 09 Sep 2021 23:12:54 GMT  
		Size: 7.1 MB (7097364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6fad868bb7f9d2057399b0e63a00ac434718e1ae15b711ebd6538230d5d15`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 1.1 MB (1120011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b390087aaec64b1435a6e47fcb0f6d5404981b9c085cc7777616075f6c7c90c4`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ce00c5fb3b7665385ce09f127bb1e442470e68e937ef6cf248affa8c5a5f2520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118449664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cfc73f626d5d8c2436225d97336f140afebc4991de582e1afd6ef5da98ee5b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:33 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:27:17 GMT
ENV GOLANG_VERSION=1.17.1
# Fri, 10 Sep 2021 00:30:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 10 Sep 2021 00:30:35 GMT
ENV GOPATH=/go
# Fri, 10 Sep 2021 00:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:30:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Sep 2021 00:30:38 GMT
WORKDIR /go
# Fri, 10 Sep 2021 01:05:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 01:05:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 01:05:36 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 01:05:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 01:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 01:05:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 01:05:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316d1588ef06afb0d7a96646bb3a1367bce295885797fd976945ed318a4eb9c`  
		Last Modified: Mon, 30 Aug 2021 21:59:27 GMT  
		Size: 281.9 KB (281927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e156a554eded13f9baa4042fb4d12b879560bebfd8aca837bf0b52669f7932`  
		Last Modified: Mon, 30 Aug 2021 21:59:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340913e3811973f494281a53e452b02a3452b65dff8016bb0281f440d907b995`  
		Last Modified: Fri, 10 Sep 2021 00:45:47 GMT  
		Size: 107.6 MB (107637928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f630dccb8f98b0e0c9749886d57178b35e57cb8190c7aae3fcb274cb0b7300`  
		Last Modified: Fri, 10 Sep 2021 00:45:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5eb1022e0b720923e3bbf90f4c4187b742dbe898fbb320597f7a6f18339d0`  
		Last Modified: Fri, 10 Sep 2021 01:06:27 GMT  
		Size: 6.7 MB (6722122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff9a04fa68552015e363e07480e2576f2c693406d1aec848a8d68661294e371`  
		Last Modified: Fri, 10 Sep 2021 01:06:26 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee0066e89945dcd9b9cd7b7fde76d311e2ba9eb2aea4a979a1127ca0da77e5`  
		Last Modified: Fri, 10 Sep 2021 01:06:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:16873cb6ebb87c355077baa9e6da4fb95ee2388105a0d152fdc47ea77e03f719
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:2.4.5-builder-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:c05c80918ab2e3bdfecd480a6ffb76a5d784d46521cc4e07d03394923cd00d48
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2858877989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bf83018c7cbfec357c464d16b8dae6a41a26166e275948ad315c0d7393ac2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:09:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:09:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:11:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:11:44 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:13:11 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:17:38 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:21:35 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:21:37 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:18:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:18:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:18:39 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:18:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:19:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:19:47 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d2bb4c99ec6467c6c9f474360867d31d27d22bc5be8432059a33a7c602a8`  
		Last Modified: Wed, 25 Aug 2021 13:38:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c31ebb0e52f79c34d0f70b88124ab4959963315dd2da2ec7117063a82d1392`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1935f777314159e43ee24dde17dba33b985a315578d33ec24796ba0ad27f679c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae930e0413fc2f7343e0b46be3ab58503ac4c137e8e6f83c7341838a22c88f3c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6bfd344bdb877d2969098eeb083c114ac4a7ef914d7dcf8eaef4d16e1e248c`  
		Last Modified: Wed, 25 Aug 2021 13:39:17 GMT  
		Size: 25.5 MB (25479918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edda6fbc32a924622fc427734f8d51447a5451f6af8f19da56ef0a27eb34e1a9`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99710b5a5f6d2c1a706493886815250b483d593751506bb096f01ef1d21fd615`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 341.4 KB (341422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4c182170aae5f94cb419bef973f17cd6202c37309480a38333e932f50d0a2a`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19d8d7117b82ef2ee7903f93b8bb7154303b39a1a414461973cf1fcec6164e`  
		Last Modified: Thu, 09 Sep 2021 21:50:44 GMT  
		Size: 145.4 MB (145374753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3826ee6919e32370009775d7e1ea3ffb058f73171f12850c81cd06d7ec08e`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa574525bddae890bf3ee7af7c9ca44962144f7369a75ca44a0c91499f0c5ea`  
		Last Modified: Thu, 09 Sep 2021 22:21:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c383c2091f6f3c8a5bb5f80daf19a417eb4d16e7388332dd8504b854c5d60d7`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca05589790af5b5a3245cb4020121cd24fa7aafcde294bc74d021e1c801f4a8`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe88d3658808037a2f2df97370e9e616f7f61c0b2c81b6fe7d69b5b7decbfda5`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7131f64e32c3073453abaaf1c693d382238a03215217f0fea25131d65252c179`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.7 MB (1665415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8844153c33fc2697353d907cf2a11433cb7d88e55361995778e61d6dc8131801`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:67f3e7cc995fb43dd91938de46517e8a19471dcc9776214d7d1c8737f0474fd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:2.4.5-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:e56175933e7ea82c7f024a59b0388740749e68a8de287a917f91faa0f5b73ff2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448258804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540f1a97650454d989940241d1e55739837273b1056174b03f9d23e6b3a03fe7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:16:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:16:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:16:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:16:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:18:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:18:14 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:19:10 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:21:49 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:25:42 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:25:43 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:20:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:20:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:20:03 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:21:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:21:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f574487f5e33222a294b80d8246d04988a26a38908346c254fa2647c5a7e028d`  
		Last Modified: Wed, 25 Aug 2021 13:39:45 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1bdad4b79465c250e34a289c1b634c4874290ec1fa9da12f91124ba323cb8`  
		Last Modified: Wed, 25 Aug 2021 13:39:44 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca6c7d62e34b14c38c401eb0e5cd89bf7ec9b271c80606691b154e354576ef`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217b8e5d43bb747a0877294acd5f9e1e22f072cc43f97874b9ecb708b70e7d96`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c80e7cfb2acdd3bfa5d45d3d78106e313290ca31797c9e09c7a33d383b758e`  
		Last Modified: Wed, 25 Aug 2021 13:40:10 GMT  
		Size: 25.4 MB (25442011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100167a51a1a9636523c0c49bf6777c5827b991a8d566c9f5d11aa1484485245`  
		Last Modified: Wed, 25 Aug 2021 13:39:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d512787c5e559f25417897aa90a76bf53bf803d34049a88a99cf226d284e96`  
		Last Modified: Wed, 25 Aug 2021 13:39:41 GMT  
		Size: 344.6 KB (344643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebb07b7d9521bf8d2019c0b625d35b815ef26420762706518f517b771a641ff`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8950c36928df1966dbd4308487add3236428fbc4bbf53c6334594fa1589ac4c1`  
		Last Modified: Thu, 09 Sep 2021 21:51:35 GMT  
		Size: 149.9 MB (149860850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51fdf50a7f76c282904490438b43225081dfe0b7965b17cbcbe5696d0f40496`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.5 KB (1519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09564a8db3d28ef4a452036d545bef45bfd9bba2ea702af06ebad5815acca1f`  
		Last Modified: Thu, 09 Sep 2021 22:22:14 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091b186c7f57f040a7c4753bc8b87fdb6c77efe558e44239c050feee6b9a994`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fe2e91a54a2f85d7d88502f47f82c0e7dc6ed3786c9e406b9577207413fdc8`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec7213f2701e2b985f6fd1d12d730aba1ca4c77ae444884b6cabc92c55d8604`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0424b377d7e54c2cf425c9ff6f65e74346d1a33383bd92568bead966ac9b89b4`  
		Last Modified: Thu, 09 Sep 2021 22:22:12 GMT  
		Size: 1.6 MB (1626867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a855cf3d4c553cd4a2241648b20fd2bbb28ce2ac481f3f20d2282aa35dbcb36`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-windowsservercore`

```console
$ docker pull caddy@sha256:c425c63e4e236cbe5bee3492948f73aa85142a1392096f56c9e952f6cfc61364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:2.4.5-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.5-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9ba0b87da005cab3abb5809cf21dc3b12f8fac8e83c43179846866ba77a9883f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:2.4.5-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.5-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:15e5d6e48e5705c59d244d4506d9259c37b03f6ce2a15bed80e02c1e533ad2ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:2.4.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:6f3b5ea2bfc0b28617452cd422177cc1bf67bd75dc1705cb863fd57d0b43faac
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
$ docker pull caddy@sha256:845a00bcc86f8ef55e3ffad434315ea3db858efb04682b6d0881606fb68de9f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14737526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a821fafa344e09dc30d1150bb619f0522186943dfbfe5d01634635c4e11c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:19:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:19:31 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:19:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:19:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:37 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d9d63a262eb117d9f55cf667904b985eb6dd9830783f17146a17a107a7ee19`  
		Last Modified: Tue, 07 Sep 2021 19:20:03 GMT  
		Size: 301.0 KB (301044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d54a459a500730b7153882903986d92e877f472e9d6ead142fab9dcb6464e1`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7c08047a89fabece2d8f1e12d68e1df255fe9c35b5975ff7a707d699359dcf`  
		Last Modified: Tue, 07 Sep 2021 19:20:06 GMT  
		Size: 11.6 MB (11616053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480638d00096415d2de6729bbcc01c75ee3ffeae1dad128c0fb0287c44185632`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:20f1145a9b70aabfa9586f75523258a4a98774618a9625cf02dc2e9c139cfd1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13952683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ef219652d94015e6f435f1d1f504736e9f4b0a0e79b1a4d532d6d18fe5fad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:49:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:49:35 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:49:41 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:49:42 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:49:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:49:48 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254033e1bbf10f9a1641b6005ee6ae290bdec377e00d2e5290e33dc0eb8f9b6`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 301.2 KB (301188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038de9754eec9aa2df09a34c0d7029c335199166de56398d21fb595fd289dd`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a15167bbb466deb6092c935cebbd9a53f872b614c83873105d590b6eb49f0ac`  
		Last Modified: Tue, 07 Sep 2021 19:51:24 GMT  
		Size: 11.0 MB (11018064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35905ee7a334ccab1c6c823badcecdd44820eb72bf4598a513885c773c44b5b`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9dfeb79eec5a0670d371d0441bb86262c154c1bc0b1b60a045698896b6dc59ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13736572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34125796b97ec78f63b7751f271503501af02ec6d00a32966d1099d71fe453e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:57:36 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:57:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:57:39 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:57:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:57:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:57:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:57:46 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:57:47 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:57:52 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:57:52 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:57:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c39987cd6455919d7455feed9aba93a44659ef658fbef5d4d52500beddac5`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 300.4 KB (300356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e223cb6b0d911c9cc6575c496bc4f96f1968db869a8a07694f3f49897920f264`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e52153d20928d86c87f7b2b39f8580cc7323e1b8a59a70936dc2aedc241489`  
		Last Modified: Tue, 07 Sep 2021 19:59:20 GMT  
		Size: 11.0 MB (10999817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231751a6396075ec359101a350a68fd144ab08e31360f7d72c1c7562f931c360`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:758247b074c2f087ee69d246b8765fb5675b6cd56a3c3ef1a5e7ce835a367e22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13654366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b4c65944934a92f9b7c40fbad35a46c8f07383af3795cada31a37f0107fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:39:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:39:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:39:28 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:39:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:39:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:39:33 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:39:34 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:39:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ceb5c04e8fd1a803328fe646ade037fd80af5d1744f9ceda93b4230e5a65b1`  
		Last Modified: Tue, 07 Sep 2021 19:40:18 GMT  
		Size: 301.2 KB (301219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ccdeb47ad54cf62b8f4b6d50208be6d2fe93d863c98e5882a78aeb226fdf1d`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f833026ad56d988c927a40940840f6a33639da2da692c23fb6d794979d6ab8a7`  
		Last Modified: Tue, 07 Sep 2021 19:40:20 GMT  
		Size: 10.6 MB (10635335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e54e7d8eca4b8cf577225887b306d095c98a1636588821fa87515405f3a7e13`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:09f31d1398820362f71bd863c8435a37aaedda9d02fe76c71ccc1c6bc62e46cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13319309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffdd09752fbe7b156120e1250d5383a3670292ae5e9a0e317883f52e732cde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:16:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:16:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:17:07 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:17:56 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:18:01 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:18:05 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:18:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:18:55 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:12 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:21 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d32e3566fcaa11540498ebdd9ecc55cd2e2dca73a6b62317657a9e75749272`  
		Last Modified: Tue, 07 Sep 2021 19:21:13 GMT  
		Size: 303.2 KB (303162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a831abca68890cbd7a89171bb93c9af5c1b102852f0f1f3326ff7c104ced90`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475efcd27e409cc064d659d255fbfb70896b95c3c36149b9a5b8d1abe86e656b`  
		Last Modified: Tue, 07 Sep 2021 19:21:14 GMT  
		Size: 10.2 MB (10197877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a9218ca8c9a1a05649cc5d0eb91f1b2985152d796a63f525c75f5380288bf8`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:d08cf598992165b333bcdea3ad215e6db5f01014f7facd1052d30674b6adbeee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14122948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d162c8bd11aec83d5d81279ca9393020c704e9629f7270c5a36067742b87caf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:41:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:41:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:41:33 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:41:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:41:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:41:49 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:41:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9c7d5d2c4319fc2386cc1a009e57751b8d7a7d807ae0e867e4d6273e06731d`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 301.5 KB (301462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c7b669e195c7cce7cf6d957130645125c1171c464622ceaa01378d18f24e37`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c91b4718f6b0100a4d5f31ab39aa7f732cb3e6d23f084e38e4918a85123a7`  
		Last Modified: Tue, 07 Sep 2021 19:42:45 GMT  
		Size: 11.2 MB (11212039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47704db6d31d2185044e1f3118b87fb2db0caa91fee7ef1cec3ec4a130ad9c`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:9c67813f5545c47b508f871e591fde6f07c649663e1f6444a39a3f78ef5edfdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:7c4854796d5ff77f514c04627f2ec1c375fada1285680273ecf06a2bc8d60cc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121056544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d72fd43a1d67a590271e3f191decedd8b71020ec56d47bb3f2fccd77f452e5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:05 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:21:07 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:22:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:22:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:22:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:22:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:22:59 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:50:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:50:58 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:50:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:50:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:51:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adcdaf11c89113a810db23d523e549d634d7de695a72b0ce98a1f912101262`  
		Last Modified: Mon, 30 Aug 2021 22:01:00 GMT  
		Size: 281.5 KB (281508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b176561691ea11cfe541f3ee363a3aa67e3649eb3273bea62ebeea713eaecd`  
		Last Modified: Mon, 30 Aug 2021 22:00:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a181aec76ea0e8e1b9ceb94467d41cab2fc9417199f12fa6fec3c50137b2933`  
		Last Modified: Thu, 09 Sep 2021 21:32:18 GMT  
		Size: 110.1 MB (110088128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e85de490b301eaafbd51e519e1bf78ed069f65b9f1735b697d139b5f62beaa`  
		Last Modified: Thu, 09 Sep 2021 21:32:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820fbf8070d3ce8dd2131897643ef5f114f3b6460df18bb30178ad42818d7895`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 6.6 MB (6626789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be64ec0930796519b26c01048a13bb77ee8567b37644a29f234f9ad1ca057c72`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 1.2 MB (1244960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c1a24ed462f4f84d50b399f1ff361c49edab51a614e1c02e171c8b1acbbe28`  
		Last Modified: Thu, 09 Sep 2021 21:51:20 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:df768c7d904cfe5f53a02be80a005731d6e73fe96c9059808dbce1c4525c9ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115536665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589c4f054797050b670d7147b81b9f77d40846a8a955fe45875b36743a901c02`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:49:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:49:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:05:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:08:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:08:48 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:08:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:08:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:08:50 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:41:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:41:50 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:41:50 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb221a547a2f49a13c3bbe14f37b0474b2066cece57c67c2fbc1fb07d89aad51`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2968f26f7f14fe309f1a7a85ad968b81a7daa93c078322a84eb5c4192326828`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9feb2689a1f4585cd8be9f2d9ebef91293de2634fb8656a34a8b6ee2a1fc955`  
		Last Modified: Thu, 09 Sep 2021 21:21:18 GMT  
		Size: 105.0 MB (104963985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c005db8fb9ff36fc9e0ce4e66886cafebecd5b7bcc46c08be65094c86e79eb`  
		Last Modified: Thu, 09 Sep 2021 21:20:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c1e636109657a0bb87f7168403a5f2364d5d4790b5b64702fcb241b841c`  
		Last Modified: Thu, 09 Sep 2021 21:43:00 GMT  
		Size: 6.5 MB (6485282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0dee99740bcf1ff7425650fd30e06d203628e08a23e53e51d4a245eec3c353`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 1.2 MB (1177568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db147b9a90d89a0071478428d882f75926adadb6b51474f7035b47e08b04b8`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:66510e6f5ac60a1293e26109be680f90c098e95f5807eb7dc1adfb5c91296d69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114434759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f52bd0e9b05ba459114822b3fed67dcedb8c5d4b7b2fadca9f8a5a24ecad3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 23:51:38 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 23:51:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 23:51:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:45:53 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:57 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:49:00 GMT
WORKDIR /go
# Fri, 10 Sep 2021 00:56:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 00:56:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 00:56:39 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 00:56:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 00:56:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 00:56:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 00:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417f62ae10851eaf03f096c21f2848fdfe2517baf1faffe0a25f4a1f9853e31`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fcbf7d3458d8a294b9a3c72856e5e7ba1372b93f8fc485abecc73f5a8c9b6`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f578778b0e30a8a96971a61afc3fc6db4d30bfa0492a2e76a7258ba63c9f30`  
		Last Modified: Thu, 09 Sep 2021 23:10:09 GMT  
		Size: 104.8 MB (104761719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93a399a67bd75c73ff72134700994ea60add14a1bd3b0d31c62d6c3ce2e2ace`  
		Last Modified: Thu, 09 Sep 2021 23:08:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfe1c03b027f77471402757e95f6f4f82c0d6cd7c4de526518112a1ba027517`  
		Last Modified: Fri, 10 Sep 2021 00:57:51 GMT  
		Size: 5.8 MB (5784816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f7b85f32126cf499c3ce4a1e59e2ad49a8b0e67dfc6ed519033f9df1ddf86`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 1.2 MB (1176262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d94d2c5711b07a6dec9f1f610397ef3ece1750d10c5f6995909f8a82e542e`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3ff72bf69ed60e7be2460e009e5482d1833613b71d61caa64b2632d1bd476b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115219439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b849c371ea6db9199f462a319cfed5552bcdce64f45ef384fd10dd659f7d5b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:41:35 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:46:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:27 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:48:28 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:38:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:38:57 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:38:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:38:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:38:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f2d53f512ea6320316a88e3c306ab2b3a98fccaeb99b4d3ae53c8bdea9e38`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 281.7 KB (281685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70ebbbe112c904d5fa82be2f7801285d376cdf6feea060292096f84b51c668`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e85633e404a49ac115564fa57298187110e7be113c5ff032acfe07513de0d9`  
		Last Modified: Thu, 09 Sep 2021 22:58:24 GMT  
		Size: 104.3 MB (104339130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fd022f582a715a4b1da40be36778771151446f39826676e5d4077c41236106`  
		Last Modified: Thu, 09 Sep 2021 22:58:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb241419bc9c911368f25f2a0f9f85d775eb785aa022f3fb742dd281f960a`  
		Last Modified: Thu, 09 Sep 2021 23:39:35 GMT  
		Size: 6.7 MB (6737938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5e29c4046768a912b16e10abad3b62e5422fc6016f2d35ecbfdd8467e6859`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 1.1 MB (1148145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6994d1faf2f00e16157a93954775e2721979285cc30b828d3814f6d1b21f7`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:9fb0df244fcc2da512b695f9d54178aa6a3536b6496b3a30ca7f23be7adac64c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114019581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa14b6844e2f03eb076817bf5c21767807433bf03846c474cb0cc74097c28b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 00:28:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 31 Aug 2021 00:29:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 00:29:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:29:06 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:31:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:31:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:32:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:32:21 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:11:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:11:34 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:11:38 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:11:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:11:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:12:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539d90ff594fe73c1a1e31b2230e539a965f33143a3c9fbd89507336ed283c2`  
		Last Modified: Tue, 31 Aug 2021 00:52:27 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a17d0ec6ff5411e524016f0ac7033cf7a0a8935f7a5e299d4d7acaad208b26`  
		Last Modified: Tue, 31 Aug 2021 00:52:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc99db09336e6fa3434452924f7d000b95f900c79247baf141252aff2663f8`  
		Last Modified: Thu, 09 Sep 2021 22:52:11 GMT  
		Size: 102.7 MB (102705568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344c38399c8dde1d0551c54c18215c10585c13293c21399eb6c0f1765384cef`  
		Last Modified: Thu, 09 Sep 2021 22:51:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8224fba31f57c4a32f77d62335f2a90f191b76b0c6377b08df77e013f969b0`  
		Last Modified: Thu, 09 Sep 2021 23:12:54 GMT  
		Size: 7.1 MB (7097364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6fad868bb7f9d2057399b0e63a00ac434718e1ae15b711ebd6538230d5d15`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 1.1 MB (1120011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b390087aaec64b1435a6e47fcb0f6d5404981b9c085cc7777616075f6c7c90c4`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:ce00c5fb3b7665385ce09f127bb1e442470e68e937ef6cf248affa8c5a5f2520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118449664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cfc73f626d5d8c2436225d97336f140afebc4991de582e1afd6ef5da98ee5b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:33 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:27:17 GMT
ENV GOLANG_VERSION=1.17.1
# Fri, 10 Sep 2021 00:30:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 10 Sep 2021 00:30:35 GMT
ENV GOPATH=/go
# Fri, 10 Sep 2021 00:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:30:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Sep 2021 00:30:38 GMT
WORKDIR /go
# Fri, 10 Sep 2021 01:05:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 01:05:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 01:05:36 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 01:05:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 01:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 01:05:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 01:05:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316d1588ef06afb0d7a96646bb3a1367bce295885797fd976945ed318a4eb9c`  
		Last Modified: Mon, 30 Aug 2021 21:59:27 GMT  
		Size: 281.9 KB (281927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e156a554eded13f9baa4042fb4d12b879560bebfd8aca837bf0b52669f7932`  
		Last Modified: Mon, 30 Aug 2021 21:59:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340913e3811973f494281a53e452b02a3452b65dff8016bb0281f440d907b995`  
		Last Modified: Fri, 10 Sep 2021 00:45:47 GMT  
		Size: 107.6 MB (107637928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f630dccb8f98b0e0c9749886d57178b35e57cb8190c7aae3fcb274cb0b7300`  
		Last Modified: Fri, 10 Sep 2021 00:45:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5eb1022e0b720923e3bbf90f4c4187b742dbe898fbb320597f7a6f18339d0`  
		Last Modified: Fri, 10 Sep 2021 01:06:27 GMT  
		Size: 6.7 MB (6722122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff9a04fa68552015e363e07480e2576f2c693406d1aec848a8d68661294e371`  
		Last Modified: Fri, 10 Sep 2021 01:06:26 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee0066e89945dcd9b9cd7b7fde76d311e2ba9eb2aea4a979a1127ca0da77e5`  
		Last Modified: Fri, 10 Sep 2021 01:06:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:c05c80918ab2e3bdfecd480a6ffb76a5d784d46521cc4e07d03394923cd00d48
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2858877989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bf83018c7cbfec357c464d16b8dae6a41a26166e275948ad315c0d7393ac2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:09:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:09:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:11:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:11:44 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:13:11 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:17:38 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:21:35 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:21:37 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:18:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:18:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:18:39 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:18:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:19:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:19:47 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d2bb4c99ec6467c6c9f474360867d31d27d22bc5be8432059a33a7c602a8`  
		Last Modified: Wed, 25 Aug 2021 13:38:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c31ebb0e52f79c34d0f70b88124ab4959963315dd2da2ec7117063a82d1392`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1935f777314159e43ee24dde17dba33b985a315578d33ec24796ba0ad27f679c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae930e0413fc2f7343e0b46be3ab58503ac4c137e8e6f83c7341838a22c88f3c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6bfd344bdb877d2969098eeb083c114ac4a7ef914d7dcf8eaef4d16e1e248c`  
		Last Modified: Wed, 25 Aug 2021 13:39:17 GMT  
		Size: 25.5 MB (25479918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edda6fbc32a924622fc427734f8d51447a5451f6af8f19da56ef0a27eb34e1a9`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99710b5a5f6d2c1a706493886815250b483d593751506bb096f01ef1d21fd615`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 341.4 KB (341422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4c182170aae5f94cb419bef973f17cd6202c37309480a38333e932f50d0a2a`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19d8d7117b82ef2ee7903f93b8bb7154303b39a1a414461973cf1fcec6164e`  
		Last Modified: Thu, 09 Sep 2021 21:50:44 GMT  
		Size: 145.4 MB (145374753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3826ee6919e32370009775d7e1ea3ffb058f73171f12850c81cd06d7ec08e`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa574525bddae890bf3ee7af7c9ca44962144f7369a75ca44a0c91499f0c5ea`  
		Last Modified: Thu, 09 Sep 2021 22:21:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c383c2091f6f3c8a5bb5f80daf19a417eb4d16e7388332dd8504b854c5d60d7`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca05589790af5b5a3245cb4020121cd24fa7aafcde294bc74d021e1c801f4a8`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe88d3658808037a2f2df97370e9e616f7f61c0b2c81b6fe7d69b5b7decbfda5`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7131f64e32c3073453abaaf1c693d382238a03215217f0fea25131d65252c179`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.7 MB (1665415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8844153c33fc2697353d907cf2a11433cb7d88e55361995778e61d6dc8131801`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:e56175933e7ea82c7f024a59b0388740749e68a8de287a917f91faa0f5b73ff2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448258804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540f1a97650454d989940241d1e55739837273b1056174b03f9d23e6b3a03fe7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:16:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:16:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:16:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:16:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:18:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:18:14 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:19:10 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:21:49 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:25:42 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:25:43 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:20:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:20:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:20:03 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:21:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:21:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f574487f5e33222a294b80d8246d04988a26a38908346c254fa2647c5a7e028d`  
		Last Modified: Wed, 25 Aug 2021 13:39:45 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1bdad4b79465c250e34a289c1b634c4874290ec1fa9da12f91124ba323cb8`  
		Last Modified: Wed, 25 Aug 2021 13:39:44 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca6c7d62e34b14c38c401eb0e5cd89bf7ec9b271c80606691b154e354576ef`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217b8e5d43bb747a0877294acd5f9e1e22f072cc43f97874b9ecb708b70e7d96`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c80e7cfb2acdd3bfa5d45d3d78106e313290ca31797c9e09c7a33d383b758e`  
		Last Modified: Wed, 25 Aug 2021 13:40:10 GMT  
		Size: 25.4 MB (25442011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100167a51a1a9636523c0c49bf6777c5827b991a8d566c9f5d11aa1484485245`  
		Last Modified: Wed, 25 Aug 2021 13:39:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d512787c5e559f25417897aa90a76bf53bf803d34049a88a99cf226d284e96`  
		Last Modified: Wed, 25 Aug 2021 13:39:41 GMT  
		Size: 344.6 KB (344643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebb07b7d9521bf8d2019c0b625d35b815ef26420762706518f517b771a641ff`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8950c36928df1966dbd4308487add3236428fbc4bbf53c6334594fa1589ac4c1`  
		Last Modified: Thu, 09 Sep 2021 21:51:35 GMT  
		Size: 149.9 MB (149860850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51fdf50a7f76c282904490438b43225081dfe0b7965b17cbcbe5696d0f40496`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.5 KB (1519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09564a8db3d28ef4a452036d545bef45bfd9bba2ea702af06ebad5815acca1f`  
		Last Modified: Thu, 09 Sep 2021 22:22:14 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091b186c7f57f040a7c4753bc8b87fdb6c77efe558e44239c050feee6b9a994`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fe2e91a54a2f85d7d88502f47f82c0e7dc6ed3786c9e406b9577207413fdc8`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec7213f2701e2b985f6fd1d12d730aba1ca4c77ae444884b6cabc92c55d8604`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0424b377d7e54c2cf425c9ff6f65e74346d1a33383bd92568bead966ac9b89b4`  
		Last Modified: Thu, 09 Sep 2021 22:22:12 GMT  
		Size: 1.6 MB (1626867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a855cf3d4c553cd4a2241648b20fd2bbb28ce2ac481f3f20d2282aa35dbcb36`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:dd81a9e615feaf5220bab8835282970fecfb2515870f1b63d3540d149855d060
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
$ docker pull caddy@sha256:7c4854796d5ff77f514c04627f2ec1c375fada1285680273ecf06a2bc8d60cc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121056544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d72fd43a1d67a590271e3f191decedd8b71020ec56d47bb3f2fccd77f452e5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:05 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:06 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:21:07 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:22:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:22:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:22:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:22:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:22:59 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:50:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:50:58 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:50:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:50:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:50:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:51:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31adcdaf11c89113a810db23d523e549d634d7de695a72b0ce98a1f912101262`  
		Last Modified: Mon, 30 Aug 2021 22:01:00 GMT  
		Size: 281.5 KB (281508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b176561691ea11cfe541f3ee363a3aa67e3649eb3273bea62ebeea713eaecd`  
		Last Modified: Mon, 30 Aug 2021 22:00:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a181aec76ea0e8e1b9ceb94467d41cab2fc9417199f12fa6fec3c50137b2933`  
		Last Modified: Thu, 09 Sep 2021 21:32:18 GMT  
		Size: 110.1 MB (110088128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e85de490b301eaafbd51e519e1bf78ed069f65b9f1735b697d139b5f62beaa`  
		Last Modified: Thu, 09 Sep 2021 21:32:03 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820fbf8070d3ce8dd2131897643ef5f114f3b6460df18bb30178ad42818d7895`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 6.6 MB (6626789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be64ec0930796519b26c01048a13bb77ee8567b37644a29f234f9ad1ca057c72`  
		Last Modified: Thu, 09 Sep 2021 21:51:21 GMT  
		Size: 1.2 MB (1244960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c1a24ed462f4f84d50b399f1ff361c49edab51a614e1c02e171c8b1acbbe28`  
		Last Modified: Thu, 09 Sep 2021 21:51:20 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:df768c7d904cfe5f53a02be80a005731d6e73fe96c9059808dbce1c4525c9ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115536665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589c4f054797050b670d7147b81b9f77d40846a8a955fe45875b36743a901c02`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:49:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:49:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:05:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:08:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 21:08:48 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 21:08:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 21:08:50 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 21:08:50 GMT
WORKDIR /go
# Thu, 09 Sep 2021 21:41:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 21:41:50 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 21:41:50 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 21:41:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 21:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 21:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 21:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb221a547a2f49a13c3bbe14f37b0474b2066cece57c67c2fbc1fb07d89aad51`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 281.7 KB (281671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2968f26f7f14fe309f1a7a85ad968b81a7daa93c078322a84eb5c4192326828`  
		Last Modified: Mon, 30 Aug 2021 22:04:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9feb2689a1f4585cd8be9f2d9ebef91293de2634fb8656a34a8b6ee2a1fc955`  
		Last Modified: Thu, 09 Sep 2021 21:21:18 GMT  
		Size: 105.0 MB (104963985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c005db8fb9ff36fc9e0ce4e66886cafebecd5b7bcc46c08be65094c86e79eb`  
		Last Modified: Thu, 09 Sep 2021 21:20:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c1e636109657a0bb87f7168403a5f2364d5d4790b5b64702fcb241b841c`  
		Last Modified: Thu, 09 Sep 2021 21:43:00 GMT  
		Size: 6.5 MB (6485282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0dee99740bcf1ff7425650fd30e06d203628e08a23e53e51d4a245eec3c353`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 1.2 MB (1177568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db147b9a90d89a0071478428d882f75926adadb6b51474f7035b47e08b04b8`  
		Last Modified: Thu, 09 Sep 2021 21:42:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:66510e6f5ac60a1293e26109be680f90c098e95f5807eb7dc1adfb5c91296d69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114434759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f52bd0e9b05ba459114822b3fed67dcedb8c5d4b7b2fadca9f8a5a24ecad3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 23:51:38 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 23:51:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 23:51:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:45:53 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:57 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:58 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:59 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:49:00 GMT
WORKDIR /go
# Fri, 10 Sep 2021 00:56:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 00:56:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 00:56:39 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 00:56:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 00:56:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 00:56:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 00:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417f62ae10851eaf03f096c21f2848fdfe2517baf1faffe0a25f4a1f9853e31`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 280.8 KB (280829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fcbf7d3458d8a294b9a3c72856e5e7ba1372b93f8fc485abecc73f5a8c9b6`  
		Last Modified: Tue, 31 Aug 2021 00:14:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f578778b0e30a8a96971a61afc3fc6db4d30bfa0492a2e76a7258ba63c9f30`  
		Last Modified: Thu, 09 Sep 2021 23:10:09 GMT  
		Size: 104.8 MB (104761719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93a399a67bd75c73ff72134700994ea60add14a1bd3b0d31c62d6c3ce2e2ace`  
		Last Modified: Thu, 09 Sep 2021 23:08:59 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfe1c03b027f77471402757e95f6f4f82c0d6cd7c4de526518112a1ba027517`  
		Last Modified: Fri, 10 Sep 2021 00:57:51 GMT  
		Size: 5.8 MB (5784816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f7b85f32126cf499c3ce4a1e59e2ad49a8b0e67dfc6ed519033f9df1ddf86`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 1.2 MB (1176262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d94d2c5711b07a6dec9f1f610397ef3ece1750d10c5f6995909f8a82e542e`  
		Last Modified: Fri, 10 Sep 2021 00:57:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:3ff72bf69ed60e7be2460e009e5482d1833613b71d61caa64b2632d1bd476b3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115219439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b849c371ea6db9199f462a319cfed5552bcdce64f45ef384fd10dd659f7d5b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:41:35 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:41:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:41:36 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:46:36 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:48:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:48:27 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:48:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:48:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:48:28 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:38:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:38:57 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:38:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:38:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:38:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:38:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f2d53f512ea6320316a88e3c306ab2b3a98fccaeb99b4d3ae53c8bdea9e38`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 281.7 KB (281685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e70ebbbe112c904d5fa82be2f7801285d376cdf6feea060292096f84b51c668`  
		Last Modified: Mon, 30 Aug 2021 21:52:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e85633e404a49ac115564fa57298187110e7be113c5ff032acfe07513de0d9`  
		Last Modified: Thu, 09 Sep 2021 22:58:24 GMT  
		Size: 104.3 MB (104339130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fd022f582a715a4b1da40be36778771151446f39826676e5d4077c41236106`  
		Last Modified: Thu, 09 Sep 2021 22:58:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb241419bc9c911368f25f2a0f9f85d775eb785aa022f3fb742dd281f960a`  
		Last Modified: Thu, 09 Sep 2021 23:39:35 GMT  
		Size: 6.7 MB (6737938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5e29c4046768a912b16e10abad3b62e5422fc6016f2d35ecbfdd8467e6859`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 1.1 MB (1148145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6994d1faf2f00e16157a93954775e2721979285cc30b828d3814f6d1b21f7`  
		Last Modified: Thu, 09 Sep 2021 23:39:34 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9fb0df244fcc2da512b695f9d54178aa6a3536b6496b3a30ca7f23be7adac64c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114019581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa14b6844e2f03eb076817bf5c21767807433bf03846c474cb0cc74097c28b3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 00:28:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 31 Aug 2021 00:29:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 00:29:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:29:06 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 22:31:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Sep 2021 22:31:58 GMT
ENV GOPATH=/go
# Thu, 09 Sep 2021 22:32:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Sep 2021 22:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Sep 2021 22:32:21 GMT
WORKDIR /go
# Thu, 09 Sep 2021 23:11:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Sep 2021 23:11:34 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 23:11:38 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 23:11:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 23:11:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Sep 2021 23:11:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Sep 2021 23:12:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4539d90ff594fe73c1a1e31b2230e539a965f33143a3c9fbd89507336ed283c2`  
		Last Modified: Tue, 31 Aug 2021 00:52:27 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a17d0ec6ff5411e524016f0ac7033cf7a0a8935f7a5e299d4d7acaad208b26`  
		Last Modified: Tue, 31 Aug 2021 00:52:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc99db09336e6fa3434452924f7d000b95f900c79247baf141252aff2663f8`  
		Last Modified: Thu, 09 Sep 2021 22:52:11 GMT  
		Size: 102.7 MB (102705568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b344c38399c8dde1d0551c54c18215c10585c13293c21399eb6c0f1765384cef`  
		Last Modified: Thu, 09 Sep 2021 22:51:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8224fba31f57c4a32f77d62335f2a90f191b76b0c6377b08df77e013f969b0`  
		Last Modified: Thu, 09 Sep 2021 23:12:54 GMT  
		Size: 7.1 MB (7097364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6fad868bb7f9d2057399b0e63a00ac434718e1ae15b711ebd6538230d5d15`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 1.1 MB (1120011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b390087aaec64b1435a6e47fcb0f6d5404981b9c085cc7777616075f6c7c90c4`  
		Last Modified: Thu, 09 Sep 2021 23:12:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:ce00c5fb3b7665385ce09f127bb1e442470e68e937ef6cf248affa8c5a5f2520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118449664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cfc73f626d5d8c2436225d97336f140afebc4991de582e1afd6ef5da98ee5b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Mon, 30 Aug 2021 21:44:33 GMT
RUN apk add --no-cache ca-certificates
# Mon, 30 Aug 2021 21:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 30 Aug 2021 21:44:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:27:17 GMT
ENV GOLANG_VERSION=1.17.1
# Fri, 10 Sep 2021 00:30:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.1.src.tar.gz'; 		sha256='49dc08339770acd5613312db8c141eaf61779995577b89d93b541ef83067e5b1'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Fri, 10 Sep 2021 00:30:35 GMT
ENV GOPATH=/go
# Fri, 10 Sep 2021 00:30:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Sep 2021 00:30:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 10 Sep 2021 00:30:38 GMT
WORKDIR /go
# Fri, 10 Sep 2021 01:05:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 10 Sep 2021 01:05:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 10 Sep 2021 01:05:36 GMT
ENV CADDY_VERSION=v2.4.5
# Fri, 10 Sep 2021 01:05:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 10 Sep 2021 01:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 10 Sep 2021 01:05:40 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 10 Sep 2021 01:05:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4316d1588ef06afb0d7a96646bb3a1367bce295885797fd976945ed318a4eb9c`  
		Last Modified: Mon, 30 Aug 2021 21:59:27 GMT  
		Size: 281.9 KB (281927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e156a554eded13f9baa4042fb4d12b879560bebfd8aca837bf0b52669f7932`  
		Last Modified: Mon, 30 Aug 2021 21:59:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340913e3811973f494281a53e452b02a3452b65dff8016bb0281f440d907b995`  
		Last Modified: Fri, 10 Sep 2021 00:45:47 GMT  
		Size: 107.6 MB (107637928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f630dccb8f98b0e0c9749886d57178b35e57cb8190c7aae3fcb274cb0b7300`  
		Last Modified: Fri, 10 Sep 2021 00:45:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff5eb1022e0b720923e3bbf90f4c4187b742dbe898fbb320597f7a6f18339d0`  
		Last Modified: Fri, 10 Sep 2021 01:06:27 GMT  
		Size: 6.7 MB (6722122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff9a04fa68552015e363e07480e2576f2c693406d1aec848a8d68661294e371`  
		Last Modified: Fri, 10 Sep 2021 01:06:26 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee0066e89945dcd9b9cd7b7fde76d311e2ba9eb2aea4a979a1127ca0da77e5`  
		Last Modified: Fri, 10 Sep 2021 01:06:25 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:16873cb6ebb87c355077baa9e6da4fb95ee2388105a0d152fdc47ea77e03f719
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:c05c80918ab2e3bdfecd480a6ffb76a5d784d46521cc4e07d03394923cd00d48
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2858877989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970bf83018c7cbfec357c464d16b8dae6a41a26166e275948ad315c0d7393ac2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:09:49 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:09:50 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:09:51 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:11:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:11:44 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:13:11 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:17:38 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:21:35 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:21:37 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:18:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:18:38 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:18:39 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:18:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:19:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:19:47 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07d2bb4c99ec6467c6c9f474360867d31d27d22bc5be8432059a33a7c602a8`  
		Last Modified: Wed, 25 Aug 2021 13:38:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c31ebb0e52f79c34d0f70b88124ab4959963315dd2da2ec7117063a82d1392`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1935f777314159e43ee24dde17dba33b985a315578d33ec24796ba0ad27f679c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae930e0413fc2f7343e0b46be3ab58503ac4c137e8e6f83c7341838a22c88f3c`  
		Last Modified: Wed, 25 Aug 2021 13:38:51 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6bfd344bdb877d2969098eeb083c114ac4a7ef914d7dcf8eaef4d16e1e248c`  
		Last Modified: Wed, 25 Aug 2021 13:39:17 GMT  
		Size: 25.5 MB (25479918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edda6fbc32a924622fc427734f8d51447a5451f6af8f19da56ef0a27eb34e1a9`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99710b5a5f6d2c1a706493886815250b483d593751506bb096f01ef1d21fd615`  
		Last Modified: Wed, 25 Aug 2021 13:38:48 GMT  
		Size: 341.4 KB (341422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4c182170aae5f94cb419bef973f17cd6202c37309480a38333e932f50d0a2a`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19d8d7117b82ef2ee7903f93b8bb7154303b39a1a414461973cf1fcec6164e`  
		Last Modified: Thu, 09 Sep 2021 21:50:44 GMT  
		Size: 145.4 MB (145374753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a3826ee6919e32370009775d7e1ea3ffb058f73171f12850c81cd06d7ec08e`  
		Last Modified: Thu, 09 Sep 2021 21:50:12 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa574525bddae890bf3ee7af7c9ca44962144f7369a75ca44a0c91499f0c5ea`  
		Last Modified: Thu, 09 Sep 2021 22:21:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c383c2091f6f3c8a5bb5f80daf19a417eb4d16e7388332dd8504b854c5d60d7`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca05589790af5b5a3245cb4020121cd24fa7aafcde294bc74d021e1c801f4a8`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe88d3658808037a2f2df97370e9e616f7f61c0b2c81b6fe7d69b5b7decbfda5`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7131f64e32c3073453abaaf1c693d382238a03215217f0fea25131d65252c179`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.7 MB (1665415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8844153c33fc2697353d907cf2a11433cb7d88e55361995778e61d6dc8131801`  
		Last Modified: Thu, 09 Sep 2021 22:21:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:67f3e7cc995fb43dd91938de46517e8a19471dcc9776214d7d1c8737f0474fd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:e56175933e7ea82c7f024a59b0388740749e68a8de287a917f91faa0f5b73ff2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6448258804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540f1a97650454d989940241d1e55739837273b1056174b03f9d23e6b3a03fe7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 13:16:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 25 Aug 2021 13:16:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 25 Aug 2021 13:16:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 25 Aug 2021 13:16:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 25 Aug 2021 13:18:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 25 Aug 2021 13:18:14 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:19:10 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Sep 2021 21:21:49 GMT
ENV GOLANG_VERSION=1.17.1
# Thu, 09 Sep 2021 21:25:42 GMT
RUN $url = 'https://dl.google.com/go/go1.17.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2f2d0a5d7c59fb38fcacaf1e272cf701bb8c050300ba8b609fc30d2c5800f02e'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Sep 2021 21:25:43 GMT
WORKDIR C:\go
# Thu, 09 Sep 2021 22:20:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Sep 2021 22:20:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Sep 2021 22:20:03 GMT
ENV CADDY_VERSION=v2.4.5
# Thu, 09 Sep 2021 22:20:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Sep 2021 22:21:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Sep 2021 22:21:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f574487f5e33222a294b80d8246d04988a26a38908346c254fa2647c5a7e028d`  
		Last Modified: Wed, 25 Aug 2021 13:39:45 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1bdad4b79465c250e34a289c1b634c4874290ec1fa9da12f91124ba323cb8`  
		Last Modified: Wed, 25 Aug 2021 13:39:44 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca6c7d62e34b14c38c401eb0e5cd89bf7ec9b271c80606691b154e354576ef`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217b8e5d43bb747a0877294acd5f9e1e22f072cc43f97874b9ecb708b70e7d96`  
		Last Modified: Wed, 25 Aug 2021 13:39:43 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c80e7cfb2acdd3bfa5d45d3d78106e313290ca31797c9e09c7a33d383b758e`  
		Last Modified: Wed, 25 Aug 2021 13:40:10 GMT  
		Size: 25.4 MB (25442011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100167a51a1a9636523c0c49bf6777c5827b991a8d566c9f5d11aa1484485245`  
		Last Modified: Wed, 25 Aug 2021 13:39:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d512787c5e559f25417897aa90a76bf53bf803d34049a88a99cf226d284e96`  
		Last Modified: Wed, 25 Aug 2021 13:39:41 GMT  
		Size: 344.6 KB (344643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebb07b7d9521bf8d2019c0b625d35b815ef26420762706518f517b771a641ff`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8950c36928df1966dbd4308487add3236428fbc4bbf53c6334594fa1589ac4c1`  
		Last Modified: Thu, 09 Sep 2021 21:51:35 GMT  
		Size: 149.9 MB (149860850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51fdf50a7f76c282904490438b43225081dfe0b7965b17cbcbe5696d0f40496`  
		Last Modified: Thu, 09 Sep 2021 21:51:00 GMT  
		Size: 1.5 KB (1519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09564a8db3d28ef4a452036d545bef45bfd9bba2ea702af06ebad5815acca1f`  
		Last Modified: Thu, 09 Sep 2021 22:22:14 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091b186c7f57f040a7c4753bc8b87fdb6c77efe558e44239c050feee6b9a994`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fe2e91a54a2f85d7d88502f47f82c0e7dc6ed3786c9e406b9577207413fdc8`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec7213f2701e2b985f6fd1d12d730aba1ca4c77ae444884b6cabc92c55d8604`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0424b377d7e54c2cf425c9ff6f65e74346d1a33383bd92568bead966ac9b89b4`  
		Last Modified: Thu, 09 Sep 2021 22:22:12 GMT  
		Size: 1.6 MB (1626867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a855cf3d4c553cd4a2241648b20fd2bbb28ce2ac481f3f20d2282aa35dbcb36`  
		Last Modified: Thu, 09 Sep 2021 22:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:ddc74d3970803736bb84cbe702d52b7800d14f54d6c0e63c2e70fdedfda05277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:845a00bcc86f8ef55e3ffad434315ea3db858efb04682b6d0881606fb68de9f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14737526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50a821fafa344e09dc30d1150bb619f0522186943dfbfe5d01634635c4e11c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:19:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:19:31 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:19:31 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:19:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:19:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:19:34 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:19:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:19:35 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:19:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:37 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:37 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:37 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d9d63a262eb117d9f55cf667904b985eb6dd9830783f17146a17a107a7ee19`  
		Last Modified: Tue, 07 Sep 2021 19:20:03 GMT  
		Size: 301.0 KB (301044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d54a459a500730b7153882903986d92e877f472e9d6ead142fab9dcb6464e1`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7c08047a89fabece2d8f1e12d68e1df255fe9c35b5975ff7a707d699359dcf`  
		Last Modified: Tue, 07 Sep 2021 19:20:06 GMT  
		Size: 11.6 MB (11616053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480638d00096415d2de6729bbcc01c75ee3ffeae1dad128c0fb0287c44185632`  
		Last Modified: Tue, 07 Sep 2021 19:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:20f1145a9b70aabfa9586f75523258a4a98774618a9625cf02dc2e9c139cfd1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13952683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ef219652d94015e6f435f1d1f504736e9f4b0a0e79b1a4d532d6d18fe5fad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:49:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:49:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:49:35 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:49:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:49:41 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:49:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:49:42 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:49:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:49:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:49:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:49:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:49:47 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:49:48 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:49:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254033e1bbf10f9a1641b6005ee6ae290bdec377e00d2e5290e33dc0eb8f9b6`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 301.2 KB (301188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038de9754eec9aa2df09a34c0d7029c335199166de56398d21fb595fd289dd`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a15167bbb466deb6092c935cebbd9a53f872b614c83873105d590b6eb49f0ac`  
		Last Modified: Tue, 07 Sep 2021 19:51:24 GMT  
		Size: 11.0 MB (11018064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35905ee7a334ccab1c6c823badcecdd44820eb72bf4598a513885c773c44b5b`  
		Last Modified: Tue, 07 Sep 2021 19:51:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9dfeb79eec5a0670d371d0441bb86262c154c1bc0b1b60a045698896b6dc59ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13736572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34125796b97ec78f63b7751f271503501af02ec6d00a32966d1099d71fe453e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:57:36 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:57:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:57:39 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:57:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:57:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:57:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:57:46 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:57:47 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:57:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:57:51 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:57:52 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:57:52 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:57:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c39987cd6455919d7455feed9aba93a44659ef658fbef5d4d52500beddac5`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 300.4 KB (300356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e223cb6b0d911c9cc6575c496bc4f96f1968db869a8a07694f3f49897920f264`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e52153d20928d86c87f7b2b39f8580cc7323e1b8a59a70936dc2aedc241489`  
		Last Modified: Tue, 07 Sep 2021 19:59:20 GMT  
		Size: 11.0 MB (10999817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231751a6396075ec359101a350a68fd144ab08e31360f7d72c1c7562f931c360`  
		Last Modified: Tue, 07 Sep 2021 19:59:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:758247b074c2f087ee69d246b8765fb5675b6cd56a3c3ef1a5e7ce835a367e22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13654366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b4c65944934a92f9b7c40fbad35a46c8f07383af3795cada31a37f0107fb7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:39:27 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:39:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:39:28 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:39:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:39:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:39:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:39:32 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:39:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:39:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:39:33 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:39:34 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:39:34 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:39:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ceb5c04e8fd1a803328fe646ade037fd80af5d1744f9ceda93b4230e5a65b1`  
		Last Modified: Tue, 07 Sep 2021 19:40:18 GMT  
		Size: 301.2 KB (301219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ccdeb47ad54cf62b8f4b6d50208be6d2fe93d863c98e5882a78aeb226fdf1d`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f833026ad56d988c927a40940840f6a33639da2da692c23fb6d794979d6ab8a7`  
		Last Modified: Tue, 07 Sep 2021 19:40:20 GMT  
		Size: 10.6 MB (10635335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e54e7d8eca4b8cf577225887b306d095c98a1636588821fa87515405f3a7e13`  
		Last Modified: Tue, 07 Sep 2021 19:40:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:09f31d1398820362f71bd863c8435a37aaedda9d02fe76c71ccc1c6bc62e46cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13319309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffdd09752fbe7b156120e1250d5383a3670292ae5e9a0e317883f52e732cde`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:16:42 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:16:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:17:07 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:17:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:17:56 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:18:01 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:18:05 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:18:12 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:18:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:18:55 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:12 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:21 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:19:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d32e3566fcaa11540498ebdd9ecc55cd2e2dca73a6b62317657a9e75749272`  
		Last Modified: Tue, 07 Sep 2021 19:21:13 GMT  
		Size: 303.2 KB (303162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a831abca68890cbd7a89171bb93c9af5c1b102852f0f1f3326ff7c104ced90`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475efcd27e409cc064d659d255fbfb70896b95c3c36149b9a5b8d1abe86e656b`  
		Last Modified: Tue, 07 Sep 2021 19:21:14 GMT  
		Size: 10.2 MB (10197877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a9218ca8c9a1a05649cc5d0eb91f1b2985152d796a63f525c75f5380288bf8`  
		Last Modified: Tue, 07 Sep 2021 19:21:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:d08cf598992165b333bcdea3ad215e6db5f01014f7facd1052d30674b6adbeee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14122948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d162c8bd11aec83d5d81279ca9393020c704e9629f7270c5a36067742b87caf`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Tue, 07 Sep 2021 19:41:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 07 Sep 2021 19:41:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 07 Sep 2021 19:41:33 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='1a19a8d94c6c16d8e671c4dad1e835e7d0d586a36e15f5300b374e5d31cf10eafdf07bc2c24d5589cdfaff1dd276e4627917802e858e14dc2351797d7dec7586' ;; 		armhf)   binArch='armv6'; checksum='5b68e8b9491507591bfa42880a771f5c687e9e081ccc249a2356b0a1cafc108214e6915d86a5342e6eb99c329942cd027bfd8960d38dae11c91a47a43926b1a8' ;; 		armv7)   binArch='armv7'; checksum='e39210f8e3634ebc85a3a32bda4bcb2263d508744f8ba3b2e9e56012cda17cabe16f2318f991e3d1d8306da49fcc2fa3bfef98f3412bbcf734376ea3bcbdf2ea' ;; 		aarch64) binArch='arm64'; checksum='da23940ff938c953d288555366e09632b31fd248e337da1990cebf0471957d14196f38396fd055d4b409f9960e2d8fb94b26ab435662a871b5ea300b9e77ad25' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='cf8d73a238628cfacea7d309f64248a6e25c76dd76a669a646845b4ca729fd677e30a2a29c75936d810b9f55df89fa17f9b6bc42c5d69e8e02b12ef4e334ad91' ;; 		s390x)   binArch='s390x'; checksum='21631de0d9c93346a9ab8658990c87bacda9c401ddb4b850a59f0c9f9665e0b93b02c0516df55eb03829f0eb5fb546683ba2d5e7b8f6174a7dfb3d13db9d81cd' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 07 Sep 2021 19:41:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 07 Sep 2021 19:41:42 GMT
ENV XDG_DATA_HOME=/data
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/config]
# Tue, 07 Sep 2021 19:41:43 GMT
VOLUME [/data]
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:41:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:41:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:41:47 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:41:48 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:41:49 GMT
WORKDIR /srv
# Tue, 07 Sep 2021 19:41:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9c7d5d2c4319fc2386cc1a009e57751b8d7a7d807ae0e867e4d6273e06731d`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 301.5 KB (301462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c7b669e195c7cce7cf6d957130645125c1171c464622ceaa01378d18f24e37`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c91b4718f6b0100a4d5f31ab39aa7f732cb3e6d23f084e38e4918a85123a7`  
		Last Modified: Tue, 07 Sep 2021 19:42:45 GMT  
		Size: 11.2 MB (11212039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47704db6d31d2185044e1f3118b87fb2db0caa91fee7ef1cec3ec4a130ad9c`  
		Last Modified: Tue, 07 Sep 2021 19:42:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:c425c63e4e236cbe5bee3492948f73aa85142a1392096f56c9e952f6cfc61364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:9ba0b87da005cab3abb5809cf21dc3b12f8fac8e83c43179846866ba77a9883f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull caddy@sha256:41e7d72dd5d9c2d1b99fcd6b39f442b38c1fd9053e616320804445a496fd7dfc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2698752341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33728bb62ba31d057027a65c26b1f5b33a5b224e49d8434da8e454d6c4bec13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:15:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:15:01 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:15:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:15:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:15:53 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:15:54 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:15:55 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:15:56 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:15:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:15:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:15:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:16:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:16:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:16:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:16:03 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:16:04 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:16:05 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:16:51 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:16:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db52efc9ab380d86f3455b420930cdfabdbeca22d84f914acb0f2471f8be0ef0`  
		Last Modified: Tue, 07 Sep 2021 19:22:36 GMT  
		Size: 390.0 KB (390026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2091af37a86f5a47cf96d7b444a9a675cff862ef313c9f510d7c5ee9630d58b2`  
		Last Modified: Tue, 07 Sep 2021 19:22:35 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeb62640fb19e1c1a5c37ca7d4215197d1447e33e15cf4ed72f0d06f88f90e1`  
		Last Modified: Tue, 07 Sep 2021 19:22:48 GMT  
		Size: 12.0 MB (12030907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dceb3620b1b7cb52b50c33651ff83beb3098d17d34255883c9af4634922989`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ece0b5c204920868fec66ff4fcef9786554e731af23f262dd3e7d6c46437fb`  
		Last Modified: Tue, 07 Sep 2021 19:22:34 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707f5a4979add68b97ef87b9855064fb18df63d953ead7070d17a6a3f784f0f`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8f83520e9e0c82a087dca427e0413a6b40b3ad36cfbe4a8b99b49f43ab80c`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c4897b905cd9545d4b80e9b5aeba737986ab3b11bd13fa9f033a1ce7a5975`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d079cd2adda08cc42898a8961c2a670f8483e2c3df52fb273f118e7bdc9c98b`  
		Last Modified: Tue, 07 Sep 2021 19:22:32 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4144405c619284d799f871a6385c61d5809b3a5f38579c4547f2823ac0bceb`  
		Last Modified: Tue, 07 Sep 2021 19:22:31 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd816209a6156d3597023439a2b194160523206a85fca0265344c0a2035688f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f4157c8edefa146c4fc3577ec4e3e4d39dfc30131f336214f1e3dae40d62b`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f356433f2b12a00a78993fd26b0ad49e3cd559938a5f8be6f12d37a4511bf10`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209d977658f6ce6cfbadb6b7208176ad6a9237bdcf310360081ad06a12eb93f`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673228ce565fb720c0dea3a729e45bb3085f0ba10d3a1c1a0c2834613a0dd165`  
		Last Modified: Tue, 07 Sep 2021 19:22:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d175be3d1e77172cd153fd9c0d2ffb9df5c6957d0a156606dfe12f350ab11f6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ccdd0eb96a950b2714725836f50789144c90ead86fcba8b66255d4b15e527d`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b7057794e3a732feeb5dea24f196da835fbcf5f48d940576086ac677f9b4d6`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b4c4b11922497df6c5ca61b891032051142a02ca6832c7015a15f131270a`  
		Last Modified: Tue, 07 Sep 2021 19:22:27 GMT  
		Size: 310.0 KB (309962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55787a3d46d3924927a25edee0165902844b360b2969997ec451e10724abd154`  
		Last Modified: Tue, 07 Sep 2021 19:22:26 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:15e5d6e48e5705c59d244d4506d9259c37b03f6ce2a15bed80e02c1e533ad2ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull caddy@sha256:fceaf27a966c473e89f49458bf63fead52804166cc2c9cd585a048b566cfc8ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283682508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa320245a9b5f8148c895b74f06d59169ef06aeb1975ce81b71476f02069f51`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 07 Sep 2021 19:17:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 07 Sep 2021 19:17:55 GMT
ENV CADDY_VERSION=v2.4.5
# Tue, 07 Sep 2021 19:18:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.5/caddy_2.4.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('794fed88b38bfeb6b3b84d63f0887c4534fc3e94bd31173182b5af80fc7783beb41192bccffdb257a9bdf59541c6822a75fdbe714d65abc3c0cce9c02018eb82')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 07 Sep 2021 19:18:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 07 Sep 2021 19:18:51 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 07 Sep 2021 19:18:52 GMT
VOLUME [c:/config]
# Tue, 07 Sep 2021 19:18:53 GMT
VOLUME [c:/data]
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.version=v2.4.5
# Tue, 07 Sep 2021 19:18:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 07 Sep 2021 19:18:55 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 07 Sep 2021 19:18:56 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 07 Sep 2021 19:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 07 Sep 2021 19:18:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 07 Sep 2021 19:18:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 07 Sep 2021 19:19:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 07 Sep 2021 19:19:01 GMT
EXPOSE 80
# Tue, 07 Sep 2021 19:19:02 GMT
EXPOSE 443
# Tue, 07 Sep 2021 19:19:03 GMT
EXPOSE 2019
# Tue, 07 Sep 2021 19:19:39 GMT
RUN caddy version
# Tue, 07 Sep 2021 19:19:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529385eeeb1211d8a8456e4d6252239f5de94512d05e4731fa148cccb9b9ac54`  
		Last Modified: Tue, 07 Sep 2021 19:23:11 GMT  
		Size: 353.0 KB (353023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0021f4c551d8537f1acb24d4c3a393af012fab25ade8fd36f57bb1369ef61c`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb2a46680ec52a939e07c8004268893dffecc5345a812793831073ecda86072`  
		Last Modified: Tue, 07 Sep 2021 19:23:23 GMT  
		Size: 12.0 MB (12035086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d65ec4ba1b2d6e4cd5bed11dbc8711197e4dc2cedf487d1556124c114aaebd`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e914c96935f4ffaf834946d17dd7a80bd8ccfd3f5c8344550c1b55d8848fa`  
		Last Modified: Tue, 07 Sep 2021 19:23:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c641a07ef51dd3f1776e5b0484cc45d095e1917b722f7df4cc1f097d6e6764`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44a70bf1e039e8c0c08962f994caf886711928e25bb6b611103a99eee9054e9`  
		Last Modified: Tue, 07 Sep 2021 19:23:08 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e24530c994428cbd8ceda3e5aae6366625a3f03e80d3aaef849c693726acd`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3630263ab48bc6f0fe3c4b3e7fd69e3406140c42002b674dcb73e5b3464ce26`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d591c1be16d8c566518b8bae46da20408802b5ec3c9e8ba730a5969d842324`  
		Last Modified: Tue, 07 Sep 2021 19:23:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8bb63b9051b8dd2fdaf7b79a33769ba36520fc31c515978fdde5f35cc4b997`  
		Last Modified: Tue, 07 Sep 2021 19:23:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89aea8755294fbffb5b885b6550eb9c1164420924bc883a267a99e7e0b2d15`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f3b28376aca4b59ac644f261fca230228d127b471bd2ea531ecba6bf6caeca`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0e5b01ac7e2a8d77ea54ce9bfa802208d2293fb588066dbad376518d8d5204`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68f5fa25fc7fd41d83f446bce0946505d5c92bddbf3cdace2899a5928d06a05`  
		Last Modified: Tue, 07 Sep 2021 19:23:05 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cc6d327cdd63af04c3e71a9285e217b5b0c5f34924795a67e7a61923a8d19`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacaa89649ec887c3648329ea4a1281e3313c6c7ec9165876cff8d5274b5f8b2`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056a51c9f4ec6572c0734e1b997435539a91d7c07b85cd19380751b07231ea46`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed784e0637e579502fe9cece14dfa6d070e3cd09843b86112e0aa7c130d958a`  
		Last Modified: Tue, 07 Sep 2021 19:23:03 GMT  
		Size: 305.0 KB (304981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a823bbbe6fd39fa6ccd4b6d33e3cd3a861eabbde8ff12b5e2d79b0bbf1049105`  
		Last Modified: Tue, 07 Sep 2021 19:23:02 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
