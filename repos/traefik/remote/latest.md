## `traefik:latest`

```console
$ docker pull traefik@sha256:b521e1ee5a19c145d153b72f8baebdad68d677ac60b6c3ff66198136ec603611
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:d16299efd58020d24b686f18a50d132ee173f6903617f884d411075d46b0a478
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29043079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ee6a3a6807db3c09e2b5752c46de57616924fca96efb0e04d46b5e477af3d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 02 Feb 2021 22:23:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.2/traefik_v2.4.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 02 Feb 2021 22:23:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 02 Feb 2021 22:23:51 GMT
EXPOSE 80
# Tue, 02 Feb 2021 22:23:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 22:23:51 GMT
CMD ["traefik"]
# Tue, 02 Feb 2021 22:23:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55558bf914b8cca4de1023d1377fd531a1ef88ed295171c52c7abbcffcae6e01`  
		Last Modified: Tue, 02 Feb 2021 22:24:21 GMT  
		Size: 25.6 MB (25556150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea38eec50335e57a2c8bfde9ac42c1222370ce3e887fd21e2ffaf05ca7364f3`  
		Last Modified: Tue, 02 Feb 2021 22:24:16 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:d8b5a6ce57328c624e7c2c1c4540ab3991e341e8b26e63ce5878f44a53422b95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27087165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:253e6b02a96a714363bad1be79c49c48287666fd89751e7146b1ad6375036a41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 02 Feb 2021 21:52:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.2/traefik_v2.4.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 02 Feb 2021 21:52:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 02 Feb 2021 21:52:27 GMT
EXPOSE 80
# Tue, 02 Feb 2021 21:52:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 21:52:28 GMT
CMD ["traefik"]
# Tue, 02 Feb 2021 21:52:29 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6105b60c39f14773e73d67adcebbea5502826654d49b130a0d44add4c3cecb77`  
		Last Modified: Tue, 02 Feb 2021 21:53:05 GMT  
		Size: 23.8 MB (23791126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d747e2d574b1c1cc065a354d904b3c42fdfd6b461fb96e3a4de958f2eecea1a8`  
		Last Modified: Tue, 02 Feb 2021 21:52:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:5bc86c671994ee7bdad7c8b350176e2ba56c3366fb422a5c7871484e2e5c83f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26708417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:207e1d0d2d5ef20d2e520edfb2d1353d1b9dc0608fb0420dbfc3b58fa036b4b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 02 Feb 2021 21:41:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.2/traefik_v2.4.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 02 Feb 2021 21:41:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 02 Feb 2021 21:41:42 GMT
EXPOSE 80
# Tue, 02 Feb 2021 21:41:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Feb 2021 21:41:43 GMT
CMD ["traefik"]
# Tue, 02 Feb 2021 21:41:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2d854741076350253739210d3eb7642de4973dd7d0193ba0259860a26d230e`  
		Last Modified: Tue, 02 Feb 2021 21:42:21 GMT  
		Size: 23.3 MB (23309587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f9704c167a30d940c894809b132160b10eabc45b63cd1d2efa073a21bd17b`  
		Last Modified: Tue, 02 Feb 2021 21:42:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
