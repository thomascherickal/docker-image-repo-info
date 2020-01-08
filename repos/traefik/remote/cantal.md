## `traefik:cantal`

```console
$ docker pull traefik@sha256:23f6057ef7b2ed7d8a36f64383c83d1639d3702d4dc8956f91b3dccc5ee9aad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cantal` - linux; amd64

```console
$ docker pull traefik@sha256:b45214fe976f562a2960b31d651937ff0b38096a5e190aa054ccd0d731c6999f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22999258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e31b6f8f937b27a5035b3783f83fdca1ed7461c8c95bfcc5b5bc437ade4edb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:34:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:34:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:34:40 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:34:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:34:40 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:34:40 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc3b9baf4c49487508fd44bf1365ad4ebb49dab85b703c52a6fff23a478411`  
		Last Modified: Tue, 07 Jan 2020 23:35:06 GMT  
		Size: 19.5 MB (19517263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62bc7f11c0b379c7d64a75606196ef30e8ca8ea737fa128f9a7ed7ce02d788`  
		Last Modified: Tue, 07 Jan 2020 23:35:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c8f068acf02c01eceac2d851e98312a29c9f0b3fa2d45e259004e869c6e5f9e3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21545654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b142df1d3f6cc564cf4ef889e8dbf1811f5a8c51d8f46ef73a1be8cc9bc8ad1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:49:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:49:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:49:54 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:49:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:49:55 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:49:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a917af9418ba8cc1c6b3c2191603a36a2f1598f152835cda15e8e8f771189a2c`  
		Last Modified: Tue, 07 Jan 2020 23:51:16 GMT  
		Size: 18.3 MB (18276155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd2532cf514fb1b82a3d6e0271ab806850c0c29b66e907f63d0d2acdedb459e`  
		Last Modified: Tue, 07 Jan 2020 23:51:09 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:29020ac8a9755056ea88c62295309cdaaa70c501d8a4976a9f8fc3f681013772
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21385632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316c3218c99d7a75e5611663f6f40751d942841d76397db294e3df7b4451f862`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:40:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:40:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:40:24 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:40:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:40:26 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:40:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed887cf3053eaa75acdc147a65a7dac09ad15b00761c6c934c452e2fd53da1f7`  
		Last Modified: Tue, 07 Jan 2020 23:41:05 GMT  
		Size: 18.0 MB (17969598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27979fd681cee9441e39782cd83d3b0483c72a311d58b9f3b31e3ba717634b88`  
		Last Modified: Tue, 07 Jan 2020 23:40:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
