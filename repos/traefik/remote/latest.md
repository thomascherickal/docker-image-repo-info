## `traefik:latest`

```console
$ docker pull traefik@sha256:c5181ddf303f1ccfd4bd6d1d9c4867b0500efb6089a0f9ccb16612438f6e934f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:a98415716a91066ef5e442969887ebb3df7d80775b5bfa7b67fcaed989833d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43232645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64586c703ab17b91788664ba464f784acd4c8058a71f54bd26852a9e6140eff5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:48:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:48:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:48:16 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:48:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:48:16 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:48:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106c23e29700a541b2b7f076be6af14e416aa36a315e95909a8f44655b2c1c6`  
		Last Modified: Wed, 06 Dec 2023 19:48:35 GMT  
		Size: 39.2 MB (39207537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc067951b11fb09519e7620e2a9a0e84e216c660aed7a38f4f3cf004354e24e1`  
		Last Modified: Wed, 06 Dec 2023 19:48:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:82aec7a0d7f4ee2d6fa39b2ec4e729fcd5fc0b7ab55eb987bc79d66fc3abbb05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40817977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7a4e3d57c06a55f5132dcc35840b0705550dbfa3a6ee98e473877671acd539`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:49:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:49:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:49:34 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:49:35 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:49:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4204dbb89422185322324d73ad620b6b37e65708e76befdc7c808a3ff33bdacb`  
		Last Modified: Wed, 06 Dec 2023 19:49:55 GMT  
		Size: 37.0 MB (37048032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1678da4540f9fd5354abf93fec0542e3639d54e99b21750e82108004a134094a`  
		Last Modified: Wed, 06 Dec 2023 19:49:49 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1f03597e0370e10e95c948a490af4ab182e9185068e212ba6e621d43f7f73ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40214807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb72c2dc074ab16d1bd1a1a657d7c8baeb8265740f81fcbab3a1a0559255e922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:54:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:54:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:54:44 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:54:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:44 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:54:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca6f355517b7c96d4dc25ab437ed008b0a935537be122866a708c2805d696d`  
		Last Modified: Wed, 06 Dec 2023 19:55:02 GMT  
		Size: 36.3 MB (36256886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0b2a752e75ae8c19870e602af930cfc9fae869f307d23ca5d36eb2528247a`  
		Last Modified: Wed, 06 Dec 2023 19:54:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:a58b6de73e9090815c8bb805c754e133f6f422f8eca41b624a5df0888cf70427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42074693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41851b5c1e5d75171cf8c53ba3350760e266d0b903787f4b2990649a48609c7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:43:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:43:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:43:47 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:43:48 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:43:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d79e9ff54bf72e763a67fc4b64f81abbe41b6854d7a90e223564c452ce7645`  
		Last Modified: Wed, 06 Dec 2023 19:44:17 GMT  
		Size: 38.2 MB (38234034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352eba91b42f08dc4d865b23f67555a4e1f0d83fc9ce83dd0705843ff49978f`  
		Last Modified: Wed, 06 Dec 2023 19:44:08 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
