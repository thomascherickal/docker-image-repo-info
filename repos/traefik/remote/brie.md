## `traefik:brie`

```console
$ docker pull traefik@sha256:c66bcedbebcf940d977409e274014285baff4e9be30abb74e1f5472c7caf9644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:brie` - linux; amd64

```console
$ docker pull traefik@sha256:1e9e2b18179e387f3a1dd69ae75e26e2ddc81dc63771ecfcbea6f4e95d050a46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29825011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65d05d7d3de78762d44e026c7562ca4c8228215c01a7241862a217e25fd8645a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 03 Aug 2021 20:31:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.0-rc5/traefik_v2.5.0-rc5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 03 Aug 2021 20:31:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 03 Aug 2021 20:31:56 GMT
EXPOSE 80
# Tue, 03 Aug 2021 20:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 03 Aug 2021 20:31:56 GMT
CMD ["traefik"]
# Tue, 03 Aug 2021 20:31:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.0-rc5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4b2f8ad060ff103cfea73f9f5ca105ef33f972f2ed27b9478147e5b0f3ee6491`  
		Last Modified: Tue, 03 Aug 2021 20:32:38 GMT  
		Size: 26.3 MB (26334187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e191a96d6c18c2ee5c85d312969c74062a00a7122a2c36cae4f3608808dc41`  
		Last Modified: Tue, 03 Aug 2021 20:32:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm variant v6

```console
$ docker pull traefik@sha256:cdcc90bffa1df6954824c9d850c1af6aeedad3531f5f275cc6b2f39459cb38cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27845657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96d367301f7e53df0bbc2a067767f7c929827798e7f8a50534a84d86fc5830b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 30 Jul 2021 17:50:16 GMT
ADD file:d8df176c5a97047d4ac655ebfc7bf2cde0a513f0120a6a7796c9724fee8acb22 in / 
# Fri, 30 Jul 2021 17:50:17 GMT
CMD ["/bin/sh"]
# Fri, 30 Jul 2021 22:26:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 30 Jul 2021 22:26:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.0-rc3/traefik_v2.5.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 30 Jul 2021 22:26:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 30 Jul 2021 22:26:37 GMT
EXPOSE 80
# Fri, 30 Jul 2021 22:26:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 30 Jul 2021 22:26:38 GMT
CMD ["traefik"]
# Fri, 30 Jul 2021 22:26:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e2a4e5657ffbdee0741d73ca6b1b16ecbc755441f7f3d8fa0365623ab5fd4544`  
		Last Modified: Fri, 30 Jul 2021 22:30:06 GMT  
		Size: 24.5 MB (24546364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0cf60f4f12ea0a2560dae4f4550722437750fe048ac9b9ac01cbf00be2be41`  
		Last Modified: Fri, 30 Jul 2021 22:29:56 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:brie` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1e5a63e52e563d0e92552f5e45c6cbdc1bbd15e0c9dc46411807a78ab4cf5ac9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27266236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fddcb7107eafc41c6b45818f3869809ea1847555b2d951bf744f70f29f160c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:15 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Tue, 15 Jun 2021 21:45:15 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:17:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jul 2021 19:04:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.5.0-rc3/traefik_v2.5.0-rc3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jul 2021 19:04:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jul 2021 19:04:39 GMT
EXPOSE 80
# Tue, 20 Jul 2021 19:04:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jul 2021 19:04:39 GMT
CMD ["traefik"]
# Tue, 20 Jul 2021 19:04:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.5.0-rc3 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b162eb5af9452c3741660adfa6fad2b853ea0249dccc6115982c64d7211e1e18`  
		Last Modified: Tue, 20 Jul 2021 19:05:54 GMT  
		Size: 23.9 MB (23863394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afc97191e1673c02ee8734e8d06db6ec74da1c5a40a2560f2065793309dbcef`  
		Last Modified: Tue, 20 Jul 2021 19:05:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
