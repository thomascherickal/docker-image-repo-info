## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:1489caffaedb09f2a9e90f85074e2330ca186dee3c151d3ab849ca74185508a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:e14a97009734c3ac7f7fbabc18cc5a068143c4e25d0d072a0d10bee2c1c7312c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f6529f13bb8557fa01f41f878e79f3714d703f4ae52d6d5c700a580877da90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:38 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:39 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d68693d54c11729ff385d1eebbcf2d487268fe3d0030be219f32ad8c717664c`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 622.4 KB (622389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2a95bcf565f364a3b5f9a4b04e21d5327717fc8241186142ea0072d1a33a84`  
		Last Modified: Thu, 15 Jun 2023 06:28:15 GMT  
		Size: 37.0 MB (36993228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bec7d4cba02c558bc5f947fbe89df277f46e49d8874185ea227323660f6ebd`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f67d07c8c40f742e8fd5b071bf8804690f631b28e9ccef7ecb9b0b6e8e3fc76c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38551154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d02830f09811f97f72174cd791d4a3781bbafe3452c20d6fcd5ed0bc09fdcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:34 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:35 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3456aa2bab6b1577d1ef938c6047142d2661cfa237d7988bc621c795148c4f9`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 624.6 KB (624561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f88f7ccafe6c44c30bccec04fdf7523c60284c5bfc2184f657e61bea7b410`  
		Last Modified: Wed, 14 Jun 2023 20:13:12 GMT  
		Size: 34.8 MB (34815309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5708ba9c2b61ea7f0086f0ef7438f9a4db8e6abbedf44bd6898d2e9ed465b`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:45bc04bd32ad505653468a88cd8afd5b9cb5d98ab85cdd2624ca31916a4baa29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37746649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4306e9b6415263e27f8f44fd3cb6a3dd2bb8c2b54f259ffde34917842ebde6c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:10:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 07:10:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 07:10:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 07:10:12 GMT
EXPOSE 80
# Thu, 15 Jun 2023 07:10:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:10:12 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 07:10:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e29fb2085d5eabaedad5069bcace309ab330ca2dc663fa75b31b1fb2bc3f62`  
		Last Modified: Thu, 15 Jun 2023 07:10:43 GMT  
		Size: 624.4 KB (624407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2eafcc680090e27cbb92458ce815a2064a02ee5e5c3410a8b0af4f0e41debd7`  
		Last Modified: Thu, 15 Jun 2023 07:10:46 GMT  
		Size: 33.9 MB (33860735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273837f3875a2b9af3ec2c0fb4a79d645e8f5b88c0379818bd3573a5ae0b3c89`  
		Last Modified: Thu, 15 Jun 2023 07:10:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:bcb98626c9002815732c2251d7ddcee0dfac94d30026478584a1ef70073947f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39660688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bbaa37db3e85f2ce21b145f541438abcca4865b961f767c68def7c13491ec1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 16:40:00 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 16 Jun 2023 16:40:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 16 Jun 2023 16:40:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 16 Jun 2023 16:40:06 GMT
EXPOSE 80
# Fri, 16 Jun 2023 16:40:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 16:40:06 GMT
CMD ["traefik"]
# Fri, 16 Jun 2023 16:40:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb0306a81fef9fd8543d89a89b4ffcc30039125cb005710104bd246877b5729`  
		Last Modified: Fri, 16 Jun 2023 16:40:37 GMT  
		Size: 622.8 KB (622767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d1a19da9d77c3c727cad72f03d4f94c36958541109e987bde688fa626e63a9`  
		Last Modified: Fri, 16 Jun 2023 16:40:43 GMT  
		Size: 35.9 MB (35862655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804c3cb633ca835d047963547d675a2e483a06537c228e5763015eda2074f6fb`  
		Last Modified: Fri, 16 Jun 2023 16:40:37 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
