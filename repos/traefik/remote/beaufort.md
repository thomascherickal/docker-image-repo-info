## `traefik:beaufort`

```console
$ docker pull traefik@sha256:db415ee1fd9cce21c192a4090101717fdc172a83a786c6a9947014cd660440cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:bf822393b55095bc13f7699ae1fa1b56bbe2e072bc2ae283bffd3a4dadd98d7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40563449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32ad70784035ddea0808eeb76e7f8a6bc64e2cb867b63c6513f8f4e853f1133`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:33 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:33 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cc32ef302c3bee4df8ba7b31c8717d000beefd7e66fbdcc07450792441ad67`  
		Last Modified: Sat, 11 Feb 2023 14:06:28 GMT  
		Size: 37.1 MB (37074888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f96cb39092b375e76e59ca53f161a1777975c9c58ea5d46e480812addb564`  
		Last Modified: Sat, 11 Feb 2023 14:06:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c6eb90c1a642c95756e04f947caee3baaed18ea1e02780df54b15240795df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a352a59877646edd78a3c6c811509111a92cd686212c584e5a5ee4845aed3818`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:21 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:22 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:23 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09007fbe2ec6b465a9c6d24d737b5f27c316d90aaae93757efb986a68a59acf9`  
		Last Modified: Tue, 14 Mar 2023 01:33:03 GMT  
		Size: 35.0 MB (34989328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ac3be21a5d5b5b332f61de0380a4216157129e1668df6f68dde1d969fb098`  
		Last Modified: Tue, 14 Mar 2023 01:32:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:49b2e1db6ca60eae983dab7632ed2ea3997c698d05dd6789eeac4de13c94ea14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b18449b8e63bade321e2c66ff5674dd5d7e3a36154f012db7b37c3c668a53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:29 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:30 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:30 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1381066f019ec8bedc5c9e8c8dcae4ed86e75cb46d22c461d5a87a060f23a`  
		Last Modified: Sat, 11 Feb 2023 06:41:17 GMT  
		Size: 34.0 MB (34023515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac00a09db30fc81aca200d38461e38fcc368b57e9878c1f51bb832b235e287d`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:e8572896cf2369e9777be7e5ce1bce0b811642e09298039e0a9d51fa570172e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39131970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194779f21f9e8eb09ec639ba646ce59761d5db6264648a5e162bf515e294517d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:38:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Mar 2023 22:38:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Mar 2023 22:38:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Mar 2023 22:38:16 GMT
EXPOSE 80
# Wed, 29 Mar 2023 22:38:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 22:38:16 GMT
CMD ["traefik"]
# Wed, 29 Mar 2023 22:38:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246408072526d1b1e0fec7aaa14e46bd07b33c86c047b5d7cdce7778f992de28`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 665.5 KB (665530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982fc64501c81b1c6a90bf3b79f669b6d16f9133509eb962541ae33f7f14c83c`  
		Last Modified: Wed, 29 Mar 2023 22:39:03 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72fc0bf978c8423d98dc56a60760c0b3d12dbea0fd1524d98a88e3f173c6ab`  
		Last Modified: Wed, 29 Mar 2023 22:38:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
