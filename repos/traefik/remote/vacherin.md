## `traefik:vacherin`

```console
$ docker pull traefik@sha256:9717bde18a6e109c63a88e4b67725500c701768d7c044fc64c83efdb892b5738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:vacherin` - linux; amd64

```console
$ docker pull traefik@sha256:c0ee1d98d82d145d449d468c9f7cecf099c224b0efa23d72f8d976548dc6ff98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d00af07cc7c91c3470ab5fb46d2caef28f984d258f110f77a7cd2b148fc93b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 20:50:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 20:50:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 20:50:14 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:50:14 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 20:50:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b54ed04da5e95dc580e80f0518e3c13b776377f5404327988acec675e499ab`  
		Last Modified: Fri, 02 Sep 2022 20:50:44 GMT  
		Size: 29.8 MB (29774829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9447aa44267fb53387d49c2e1fc049f08581306fca07488baab643e3f559d90b`  
		Last Modified: Fri, 02 Sep 2022 20:50:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:524dea2468148d17e36e8685b1ae6bb8b32fc824dc67d9ae0d006f78c205c9ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31406635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a470b476d302ab7cd2965d189b989a1ebeafc3b3f51c3fc9a3f7352590ad8c75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 19:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 19:49:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 19:49:39 GMT
EXPOSE 80
# Fri, 02 Sep 2022 19:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 19:49:39 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 19:49:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2184ddf72fafdec856907308b0832d0cb9fa3f18d27bc8923d31bf537000722a`  
		Last Modified: Fri, 02 Sep 2022 19:50:45 GMT  
		Size: 28.1 MB (28089099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bab47ff3f98940f7fa7d3eb55a81c68ba899a88b3b57e7e2ff3574eb5c2ca5`  
		Last Modified: Fri, 02 Sep 2022 19:50:39 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3af1ee8b3fff09a9e7bc958150245c14eebf6910fee151320b716a0ce0278b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30575438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148847c384149af925afcbbf2a63d3d9537e1c3e0e3fc4778ce849c30fc414a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:02:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:02:08 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:02:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:02:10 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:02:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c95a60d9885fe2865b5aef2abf3c8e02dbfcd48f4b9978e47205d35c9a2c1`  
		Last Modified: Wed, 10 Aug 2022 06:12:12 GMT  
		Size: 682.4 KB (682395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c489cee492d2fe706c61d150982ab2113f63f0b0325eecfcc529c715a025de`  
		Last Modified: Fri, 02 Sep 2022 21:03:03 GMT  
		Size: 27.2 MB (27174235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23e7c7b06001a1723b46152cba68a658ef913e0fcd9ce6a675782ee6e91153`  
		Last Modified: Fri, 02 Sep 2022 21:02:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; s390x

```console
$ docker pull traefik@sha256:0ae44e1db4e8692764f89bc9c6713b5a8f2454a49fb958670f1ce097d771f2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31970417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907601fe3e786e8291296b20b082a843538ba24e2cb77764166e496ec811d23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:18:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:19:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:19:03 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:19:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:19:04 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94fe8753c6b15e6f67f3ca19edd0d0c2c0d8f6596878b0a6e212d71d3ae470d`  
		Last Modified: Wed, 10 Aug 2022 05:50:57 GMT  
		Size: 686.5 KB (686528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fc896b96c1b9c8a8c7d6ab0cec469b6114d366b8cc7732f19d5913ad818d1`  
		Last Modified: Fri, 02 Sep 2022 21:19:39 GMT  
		Size: 28.7 MB (28677434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0189892c09ebd907a8f9e1885c492cd37742dd2d614b034515e31dda3ec17`  
		Last Modified: Fri, 02 Sep 2022 21:19:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
