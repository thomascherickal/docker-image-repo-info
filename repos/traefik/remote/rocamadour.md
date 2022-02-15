## `traefik:rocamadour`

```console
$ docker pull traefik@sha256:e88f389b79b2c287650d11751e3375ece8c5e21bd77100a22e7d0ded2a457d6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:rocamadour` - linux; amd64

```console
$ docker pull traefik@sha256:79b4af2f1a73345d9cbfc3ae9fca0bde3aaa88787d890456f312c461bc8dcdf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30343676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eddc86c9f0a0e20b8f8685faf0256cc709a28245b515967dc89a87a887f590ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:23:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 14 Feb 2022 20:35:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 14 Feb 2022 20:35:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 14 Feb 2022 20:35:18 GMT
EXPOSE 80
# Mon, 14 Feb 2022 20:35:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 14 Feb 2022 20:35:19 GMT
CMD ["traefik"]
# Mon, 14 Feb 2022 20:35:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1084cd799816f7a030d5c7985d2b38853f5ad434ee8ee15f2993cd000e5bbd`  
		Last Modified: Sat, 13 Nov 2021 07:24:22 GMT  
		Size: 677.8 KB (677824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a2034f7fb737bb150b572407f4b1e98f46082137d90237c0d6e1c6fb0195fe`  
		Last Modified: Mon, 14 Feb 2022 20:35:48 GMT  
		Size: 26.8 MB (26842503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a5f273cd24dda64deed96070fa99d8e31147bd9ebc2395f9b1f765ff8b3071`  
		Last Modified: Mon, 14 Feb 2022 20:35:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:rocamadour` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9c248cbc8c7f53de29903b1875a6d188e736916a0ef040e18707279993f39fe9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28508934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fdc7955f98c65a063a9ad35cf26ad80d6fee6ef897cf59cc1b8706bcdd66358`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:51:34 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 14 Feb 2022 19:49:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 14 Feb 2022 19:49:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 14 Feb 2022 19:49:51 GMT
EXPOSE 80
# Mon, 14 Feb 2022 19:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 14 Feb 2022 19:49:52 GMT
CMD ["traefik"]
# Mon, 14 Feb 2022 19:49:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b00cdbc51db9651a9c09390b641face7e18e642e3ff49397c6d477c89c3d7e`  
		Last Modified: Sat, 13 Nov 2021 06:54:26 GMT  
		Size: 683.0 KB (682972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3794250fa4899ce360ba5ae6150b832eb727d241cc942e1de6ec24cbc4439c3e`  
		Last Modified: Mon, 14 Feb 2022 19:51:59 GMT  
		Size: 25.2 MB (25190202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3759f754cb8220815d45d4e45fc424c3c95b471df88ae5530dfc4d6fe0fd3a`  
		Last Modified: Mon, 14 Feb 2022 19:51:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:rocamadour` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4412e77270d7f7309214c89912ba5032900a8133769fbd040d850fb485d41099
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27881402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e0c38ff9051d76cd4ee75269910ab0daccc3186b322908f9c076e3c1d54fab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:16:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 14 Feb 2022 19:57:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 14 Feb 2022 19:57:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 14 Feb 2022 19:57:27 GMT
EXPOSE 80
# Mon, 14 Feb 2022 19:57:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 14 Feb 2022 19:57:29 GMT
CMD ["traefik"]
# Mon, 14 Feb 2022 19:57:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cc5a4b7f102f236064e4712164f29c52d256612820409cc28c41a7f5def4a5`  
		Last Modified: Fri, 12 Nov 2021 18:17:40 GMT  
		Size: 680.0 KB (680008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fca17f183490f48f55763fd7a0cc5e048188f9417d11364d2326c508eba8889`  
		Last Modified: Mon, 14 Feb 2022 19:58:23 GMT  
		Size: 24.5 MB (24483326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5e8bc750970cb5bd7abf94661d4d9ea8b6a6eff513fc1906401c55e0d4bb56`  
		Last Modified: Mon, 14 Feb 2022 19:58:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
