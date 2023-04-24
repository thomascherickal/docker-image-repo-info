## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:754a02d1d0f52b0e1b9c627b42d14d92f95ab97f7666cb03499a0ca67f697b59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:369a4f37fd35962e43a93babc7eda11a57bd74fc710bb3aeea0c3b785c867b9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ac3f0a4d8ca113e05aea00346a21ed79da3038d62523f431d6aeb7d444598e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 24 Apr 2023 20:42:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0/traefik_v2.10.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 24 Apr 2023 20:42:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 24 Apr 2023 20:42:23 GMT
EXPOSE 80
# Mon, 24 Apr 2023 20:42:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:42:24 GMT
CMD ["traefik"]
# Mon, 24 Apr 2023 20:42:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8874d609a28b10481ca19277f8a43bd16f6f27ccfced2d556ee13df1437f0c`  
		Last Modified: Mon, 24 Apr 2023 20:42:49 GMT  
		Size: 37.0 MB (36992936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2e1aa05c967d3e07de6c7571c77d57f1f8c75e7515acad850f41883bc497d3`  
		Last Modified: Mon, 24 Apr 2023 20:42:43 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:6de72d501b04e2c05c29a31ea049594a241304d0e75965c8a0df3e2e79675ba4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.5 MB (38549143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574fa1a1858cc72cb1bc5c007d99a468ab591c7569a8aab3ea17e0b7b6d0e494`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:39 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Apr 2023 22:49:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Apr 2023 22:49:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Apr 2023 22:49:28 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:49:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Apr 2023 22:49:28 GMT
CMD ["traefik"]
# Fri, 07 Apr 2023 22:49:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eb72050bf74c68d6b8ca4b4f057628cfcf24a9ebf3c88aaa441cdb2ef550159e`  
		Last Modified: Fri, 07 Apr 2023 22:49:54 GMT  
		Size: 34.8 MB (34813548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c386a9784949f2cb675965bc8c2297e24fa318c62ac0f90a5a068544fe2854`  
		Last Modified: Fri, 07 Apr 2023 22:49:47 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:5d6553f78fd6138d52f1e78decf56cbe5a804c752ae5823b8ab7398e2ef11111
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37747994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa528079f2fc4543c25aa2b1a8093ad676559256e926c6b6e4c5c729ccf964db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 24 Apr 2023 20:46:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0/traefik_v2.10.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 24 Apr 2023 20:46:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 24 Apr 2023 20:46:57 GMT
EXPOSE 80
# Mon, 24 Apr 2023 20:46:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:46:57 GMT
CMD ["traefik"]
# Mon, 24 Apr 2023 20:46:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9748dafc7933375d13abf1aa50e924a2f344fab68864335b04b9566c18e9a69`  
		Last Modified: Mon, 24 Apr 2023 20:47:18 GMT  
		Size: 33.9 MB (33861568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a8ad33c596a0c20c8d75a68e3b38dffdd0442bd2d21a363fc667d88d08d1c6`  
		Last Modified: Mon, 24 Apr 2023 20:47:14 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:d0c254b6f0aa5d3567ec571d47af9b3eefdeb7ca727e2521a8b9a0ced6c11004
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39654377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d60e52bfc7696d00c2b47e7370231b7840cdabb7d1477c097e165643459ab5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Apr 2023 22:42:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.0-rc2/traefik_v2.10.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Apr 2023 22:43:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Apr 2023 22:43:01 GMT
EXPOSE 80
# Fri, 07 Apr 2023 22:43:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Apr 2023 22:43:01 GMT
CMD ["traefik"]
# Fri, 07 Apr 2023 22:43:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8b6f52b2c5da630a2545874f7e8434c96a8f927f67e153ac56d993d71d153f76`  
		Last Modified: Fri, 07 Apr 2023 22:43:25 GMT  
		Size: 35.9 MB (35856239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c7dc4bd54ad50df7a93f371fa74e83b872596728d9292f7b34943506e31d6d`  
		Last Modified: Fri, 07 Apr 2023 22:43:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
