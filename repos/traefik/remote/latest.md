## `traefik:latest`

```console
$ docker pull traefik@sha256:234df709c407306a4b7ce3f323aee24602429ea8299e6416441fc7309ac85178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:d6039a8a87021d99b45aafdad699e63fbf388917d2e934e66e20d9e46854ba6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28049629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de1a7c9d5d63d8ab27b26f16474a74e78d252007d3a67ff08dcbad418eb335ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 16 Aug 2021 19:20:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.14/traefik_v2.4.14_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 16 Aug 2021 19:20:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 16 Aug 2021 19:20:55 GMT
EXPOSE 80
# Mon, 16 Aug 2021 19:20:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 16 Aug 2021 19:20:55 GMT
CMD ["traefik"]
# Mon, 16 Aug 2021 19:20:55 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.14 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abdcd3bb40ca29c232ad12d1f2cba6efcb28e8d8ab7e5787ad2771b4e3862b0`  
		Last Modified: Mon, 16 Aug 2021 19:21:31 GMT  
		Size: 24.6 MB (24558804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4701c53ae539044a129428575f42a0e0aa5e923d04b97466915bf45f5df0e3`  
		Last Modified: Mon, 16 Aug 2021 19:21:27 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:20e664ac09630f6ba4f32bc839f8e1efdb427ebe7cd75348613592cc4e71a93b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27283972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab688756051d9aed9cb19b243da1d0f52309ba86f650ef9398cfedabc8241218`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 30 Jul 2021 17:50:16 GMT
ADD file:d8df176c5a97047d4ac655ebfc7bf2cde0a513f0120a6a7796c9724fee8acb22 in / 
# Fri, 30 Jul 2021 17:50:17 GMT
CMD ["/bin/sh"]
# Fri, 30 Jul 2021 22:26:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 17 Aug 2021 19:02:22 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.0/traefik_v2.5.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 17 Aug 2021 19:02:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 17 Aug 2021 19:02:23 GMT
EXPOSE 80
# Tue, 17 Aug 2021 19:02:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 Aug 2021 19:02:24 GMT
CMD ["traefik"]
# Tue, 17 Aug 2021 19:02:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1a82e2abdb8183eef16afe6d45e16c1b000a908fe3f8fcd17adef7778ecb37d9`  
		Last Modified: Wed, 14 Apr 2021 18:50:45 GMT  
		Size: 2.6 MB (2621912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed02d963bbf86d6e5434c3d67ade07a501b2cbc61b6ae18dfc155ede8f3b1591`  
		Last Modified: Fri, 30 Jul 2021 22:29:56 GMT  
		Size: 677.0 KB (677014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef9dfd1189f283d8da0d5fd67120c05f8bfb2ce92620208cbfe36a1e96b07d3`  
		Last Modified: Tue, 17 Aug 2021 19:04:27 GMT  
		Size: 24.0 MB (23984678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b981c2693856e1c4d582cfe2c9ef49b4a6d43ef8cc6c59c3752332c0e995e`  
		Last Modified: Tue, 17 Aug 2021 19:04:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9506435ce3d83eb9c00ffab7a98a144e06b52fe7b8af47a9fda7e1b344e30192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26720807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8479f0715ebb5225f00ed07a54d38230c38685ce2ad6d98e078d43d71a1ccf23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:15 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Tue, 15 Jun 2021 21:45:15 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:17:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 18 Aug 2021 10:13:19 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.0/traefik_v2.5.0_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 18 Aug 2021 10:13:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 18 Aug 2021 10:13:19 GMT
EXPOSE 80
# Wed, 18 Aug 2021 10:13:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 10:13:20 GMT
CMD ["traefik"]
# Wed, 18 Aug 2021 10:13:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.0 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb39c774f8e6176a8c3728cde4ec4fc741ab8ff2040415b9f55bbd839dc73b78`  
		Last Modified: Wed, 16 Jun 2021 11:18:33 GMT  
		Size: 675.5 KB (675546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f27a9ad3b6b689c8e8650d199203c67c25c3e774f6abee7eef778d8c6bc1630`  
		Last Modified: Wed, 18 Aug 2021 10:14:18 GMT  
		Size: 23.3 MB (23317965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75692599c5b083a0cff18f6d27ccd62cf653949459a71fd44f295175936cbbb6`  
		Last Modified: Wed, 18 Aug 2021 10:14:14 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
