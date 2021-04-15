## `traefik:livarot`

```console
$ docker pull traefik@sha256:08d8a7759f5fffa2441488151cedcd4d556c1f124c097f929f469c1f7b82c16f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:4e2da005d39daa3823c6930cfb4ff5eb8d75be3679a2173489d8579e655be4be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27828337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaf4b1027ed4bce7d3a15a22a7ff5f5fab274bffde1709ae85e93f15085ad98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:04:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:04:48 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:04:49 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:04:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:acb62688737133737535c58e692b79b70843447464a3760d37d1d65c33fa1e5c`  
		Last Modified: Thu, 15 Apr 2021 03:06:03 GMT  
		Size: 24.3 MB (24337513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6d79f94aac9a1ec9746826d0fd58ea98a05df8f5ed882819626db57909331`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:076ae4bba5142b3f4165a4d4ee27ab44241e1887305ddeab308242505248697c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26026374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03ac7137f8eb9cd0b2aed48106d54539242b397586fb9a2bb5f830ac68c1f871`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:58 GMT
ADD file:d8df176c5a97047d4ac655ebfc7bf2cde0a513f0120a6a7796c9724fee8acb22 in / 
# Wed, 14 Apr 2021 18:49:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:13:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 06:14:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 06:14:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 06:14:07 GMT
EXPOSE 80
# Thu, 15 Apr 2021 06:14:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 06:14:09 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 06:14:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1a82e2abdb8183eef16afe6d45e16c1b000a908fe3f8fcd17adef7778ecb37d9`  
		Last Modified: Wed, 14 Apr 2021 18:50:45 GMT  
		Size: 2.6 MB (2621912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888290a6b02b8e0b04a3589f86c5a961837ceaf0253810dacb6d6b1a1d1c6593`  
		Last Modified: Thu, 15 Apr 2021 06:15:33 GMT  
		Size: 677.0 KB (676987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe7017b46faf55abca2e5999294e972efd7320a0d12e34a09cac8178196f65`  
		Last Modified: Thu, 15 Apr 2021 06:15:43 GMT  
		Size: 22.7 MB (22727106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df17fd49c96f2bd27a92eb45fcf846ac97bdd70e64df5908a9c30dc23f11940f`  
		Last Modified: Thu, 15 Apr 2021 06:15:33 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3ac00a4751157d604689d4dd0e880cbdba19eaeee7105e1a811c735a0d152465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25476541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4a19369dcb8dfb04b19c03d97b565462c267c62458aad336915335272043c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 18:43:05 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Wed, 14 Apr 2021 18:43:06 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:07:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 08:07:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 08:07:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 08:07:36 GMT
EXPOSE 80
# Thu, 15 Apr 2021 08:07:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 08:07:38 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 08:07:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a748d105a321ac0423a9fc448ff1cc17fb6823a32bcce7e101019a84271eb2`  
		Last Modified: Thu, 15 Apr 2021 08:11:41 GMT  
		Size: 675.5 KB (675526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bd63a53d89bf73119ca1dc3301514803c1fc03f85053b78fe41c144b290e45`  
		Last Modified: Thu, 15 Apr 2021 08:11:48 GMT  
		Size: 22.1 MB (22073719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ccb8d240256ef37f70b9924731416f3a648f142403e45bd31b8eec1f897dee`  
		Last Modified: Thu, 15 Apr 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
