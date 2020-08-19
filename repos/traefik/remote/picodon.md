## `traefik:picodon`

```console
$ docker pull traefik@sha256:302e1214da614f62b8cdc930daf285bc9d8165ac15e0953309161de06a589fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:picodon` - linux; amd64

```console
$ docker pull traefik@sha256:3f5c5a46ccff636a9e726961f123638bd6854191040072d860fc15bbcee3e184
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28052206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926633bd017b112d1ee29780353bd3898e2f5f4a3b4749e8c4070ab765708bc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:33:28 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:12:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:12:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:12:05 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:12:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:12:05 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:12:05 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16506d32a25436b458a7f443ec1ca0d096d99d3479523c92c247856fc6148c0`  
		Last Modified: Fri, 24 Apr 2020 17:34:15 GMT  
		Size: 694.1 KB (694148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8843362db2d6c7cba5a5ac00938528154d1b876fe944ae136e0c6cd5d390e4f4`  
		Last Modified: Wed, 19 Aug 2020 21:12:38 GMT  
		Size: 24.5 MB (24544374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685edc151199f805d0e1910cd68e68161fbc81369caf76102ebed3176760a338`  
		Last Modified: Wed, 19 Aug 2020 21:12:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c85e11c5d0332ddc75b8a70c5fcd19540794ae68a86df0fb7c957fec76074a65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.2 MB (26178413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6d814c93b2dcc172081103002e7c5ff94bd1b8fec1210b28caca91353fdb66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:36:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 19 Aug 2020 21:04:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc4/traefik_v2.3.0-rc4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 19 Aug 2020 21:04:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 19 Aug 2020 21:04:09 GMT
EXPOSE 80
# Wed, 19 Aug 2020 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 19 Aug 2020 21:04:12 GMT
CMD ["traefik"]
# Wed, 19 Aug 2020 21:04:15 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a36cf46e6cb6a8028db7cb68482816e710935254a7d463897840713066cf5ba`  
		Last Modified: Thu, 23 Apr 2020 22:39:24 GMT  
		Size: 698.1 KB (698086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d52f51ca6c71d0c3f5144f84c3099bd4831769fa83c8d072c6b67b89c61321`  
		Last Modified: Wed, 19 Aug 2020 21:04:59 GMT  
		Size: 22.9 MB (22860023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497bf20f1fdcc8800a01dd9f26e77ac3f1236f6627bbd64100ec7926f84e2c2`  
		Last Modified: Wed, 19 Aug 2020 21:04:52 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:14b29b6c8bd7c722e1dd0e06f9f0a7e37db3a5d8467496cfde55b13073656702
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27754805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bce20c5287082213e632bc7034a39e3e84efd677922b395fd4c5d13843dfa62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:14:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 28 Jul 2020 23:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.3.0-rc3/traefik_v2.3.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 28 Jul 2020 23:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 28 Jul 2020 23:49:56 GMT
EXPOSE 80
# Tue, 28 Jul 2020 23:49:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Jul 2020 23:49:57 GMT
CMD ["traefik"]
# Tue, 28 Jul 2020 23:49:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff968af61b86e34dc2412293ade430f77b7db53f7f4adb925fec30d3ccbb2876`  
		Last Modified: Fri, 24 Apr 2020 12:43:42 GMT  
		Size: 696.1 KB (696058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32d16371e8f6c49f7eb4c9ae55be6a35d152399c37508b5a81eb631bdd0f182`  
		Last Modified: Wed, 29 Jul 2020 00:01:25 GMT  
		Size: 24.3 MB (24333955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bbea951e4557c6db83dc8f3fa25298592630e9292fe53c8f4ebcadce74658b`  
		Last Modified: Wed, 29 Jul 2020 00:01:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
