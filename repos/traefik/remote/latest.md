## `traefik:latest`

```console
$ docker pull traefik@sha256:b0e4c5d21dfd58478272d81fdb3ee4f032b738fe24260aeeb4fdb8c30168724f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:f77782c1c613d08aabe67413e2ab34a20d18a424779be6802868eb90d7c1b2eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3ef29ff3457efbc81bd711e18c29898902f608c21fc21928d43640aa00d74a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 01:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 01:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 01:39:31 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 01:39:31 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 01:39:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517a5c81aa99d6c7b3f5ba63d79cf9b29dcad97262ecace92ed87a033b9d3f3`  
		Last Modified: Wed, 24 Mar 2021 01:40:03 GMT  
		Size: 24.3 MB (24337512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6216d750eb51a362ec1238b390c1d4f3d67fe760d7519b18cc734241057d6b`  
		Last Modified: Wed, 24 Mar 2021 01:39:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:36bdc8b0f979eec6df4e0e48a10cb03d06122760428cae889dd33185b7eaa50b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cde150cf56c858ae139d9eb5aec198367c7ff2391b6f51e17c2039914fa8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 02:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 02:29:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 02:29:22 GMT
EXPOSE 80
# Wed, 24 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 02:29:23 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 02:29:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fdec5ae7c7320d5327a0bdac6ecc6a94a3f358a45742c63f49bffe7da6cfb2`  
		Last Modified: Wed, 24 Mar 2021 02:30:02 GMT  
		Size: 22.7 MB (22727107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa947f44a6dc4bfa180888f202ded6f0dba5e77a1967e6c9c30244091b2b338`  
		Last Modified: Wed, 24 Mar 2021 02:29:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9bb3516baf888fa5c81008c445ff63804f556ff68fee752a8c17fc8a8150db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1089720f9d91464f0161c603353bab15f2014e49e5228e134abae8bb3812600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:09 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:11 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf36803d5e7ca9b3042d1847d12ee10baacbcf8e84b0aad89b7d9267714e29`  
		Last Modified: Fri, 26 Mar 2021 08:11:47 GMT  
		Size: 22.1 MB (22073745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95742e6b158cadc348dddbb20aa9c7461bfe1441a1f5f3171117ac99538428`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
