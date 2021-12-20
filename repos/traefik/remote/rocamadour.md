## `traefik:rocamadour`

```console
$ docker pull traefik@sha256:2acb3fc3b15a83f7489202cf94d13baeea70212d87fb3789046c7ef014803952
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `traefik:rocamadour` - linux; amd64

```console
$ docker pull traefik@sha256:d65d0be92a53c004a163cb35e4c0c31a58edebcef1de496a319b028fa2bd09a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.2 MB (30168792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68c77ac9166db72d9e4f271680b434cb985f4659125da1c2222034612341133`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:23:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 20 Dec 2021 19:20:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.0-rc1/traefik_v2.6.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 20 Dec 2021 19:20:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 20 Dec 2021 19:20:01 GMT
EXPOSE 80
# Mon, 20 Dec 2021 19:20:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Dec 2021 19:20:01 GMT
CMD ["traefik"]
# Mon, 20 Dec 2021 19:20:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:d95732e323f1180b16089b3709e32acdd925d45c058c88e3fd9a278f8ebf095a`  
		Last Modified: Mon, 20 Dec 2021 19:20:37 GMT  
		Size: 26.7 MB (26667619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37884b0fee928687a29eb238763446dec983cdb4b55cca61344a6b6b3d5a8739`  
		Last Modified: Mon, 20 Dec 2021 19:20:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
