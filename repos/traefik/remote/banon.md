## `traefik:banon`

```console
$ docker pull traefik@sha256:9caef29a180312621550d64e9a7b736ea72f25aa22a711a8365cb4e65fdac25a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:banon` - linux; amd64

```console
$ docker pull traefik@sha256:d1317cf3bd8e5016db5f48bfc227d0e0c1d9308cf3bf7c8bc6a2e0c8e084e5ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39614731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3019f7419217f4bca7942871abea2a289dc4b55ce05eece966740497dddd4c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Tue, 21 Mar 2023 20:20:09 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 21 Mar 2023 20:20:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 21 Mar 2023 20:20:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 21 Mar 2023 20:20:12 GMT
EXPOSE 80
# Tue, 21 Mar 2023 20:20:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Mar 2023 20:20:13 GMT
CMD ["traefik"]
# Tue, 21 Mar 2023 20:20:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae84fc17309bb4699abd282faa21aee64a99f3df7bb0d6aa950911f29b7add`  
		Last Modified: Tue, 21 Mar 2023 20:20:33 GMT  
		Size: 622.9 KB (622941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a996fe26bc3c22f7e278385b1c7862a3b602c0b0d9160434f3b3289da92aeaf`  
		Last Modified: Tue, 21 Mar 2023 20:20:38 GMT  
		Size: 35.6 MB (35616976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc083908edbac98ae426bbdcdce3368ddd2b0fe34e0189d87e80ce54072b344`  
		Last Modified: Tue, 21 Mar 2023 20:20:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:10b691b83d9ed9bac5ac8d7c37c79398bfec79e73c5b7882a6d6da069d3eb277
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37252169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a74fe8cbe09d9e0c7f9f1f5eae5d4c1ce1a39daf65907779900cdce45c36ed4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 00:39:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 00:39:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 00:39:44 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 00:39:44 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 00:39:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bd7901efecc8425b6d98584a9ee5d091a238a8936fb50b8aa4654afb90d05d`  
		Last Modified: Thu, 30 Mar 2023 00:41:05 GMT  
		Size: 624.4 KB (624425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d6063123b03962a02bfe27e1157e7a846da318f6438997b771048f14b7cc0b`  
		Last Modified: Thu, 30 Mar 2023 00:41:10 GMT  
		Size: 33.5 MB (33516575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f46160874c0a777742654e0fd3a6789ac1b431552c3e2c875c39273c198f54`  
		Last Modified: Thu, 30 Mar 2023 00:41:04 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4f9029190d2211977970c56ebfa5fd21c1b32b7de344665fb0c1c3848055460e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36496410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbec9db2728fd3471e17d2dce1e771b59922d56183f86fb28b17559c86e77844`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Tue, 21 Mar 2023 20:34:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 21 Mar 2023 20:34:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 21 Mar 2023 20:34:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 21 Mar 2023 20:34:34 GMT
EXPOSE 80
# Tue, 21 Mar 2023 20:34:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Mar 2023 20:34:34 GMT
CMD ["traefik"]
# Tue, 21 Mar 2023 20:34:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38fa8056026d2f43828b73e0ab328da2596a91223ac4c6ae73fef33ff33a318`  
		Last Modified: Tue, 21 Mar 2023 20:34:50 GMT  
		Size: 624.9 KB (624926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7de9d521520dc972618c023825b448a2304fb9c7130162d42f08d8256dac98`  
		Last Modified: Tue, 21 Mar 2023 20:34:54 GMT  
		Size: 32.6 MB (32609156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0653653cea54a5782ad23bc418616e571bb4e3467e36f548b8c9bda1ad1ea35f`  
		Last Modified: Tue, 21 Mar 2023 20:34:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; s390x

```console
$ docker pull traefik@sha256:a4e2b23ab0e116c6c63eb883e41b410879f8ce7ba0705f343cac8711cfb716fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38327529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0140a070a5b28be241ddcb7b569ab11635cc2f95065d7c38d10085dbd4b8bd9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:27 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:27 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096a495bd82a55e97c5be084787578b5b5af0321a33c70ccf19bca0dc260a981`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 622.6 KB (622584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f26afb3e4c2022602d8a38957a1218703bec9d64167ba3d830a0d7216bf8f02`  
		Last Modified: Wed, 29 Mar 2023 22:39:17 GMT  
		Size: 34.5 MB (34529391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f96123c52fa98b6189d9190c14398bee66527d253e31488dc4ce2abd7f62881`  
		Last Modified: Wed, 29 Mar 2023 22:39:11 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
