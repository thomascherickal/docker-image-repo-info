## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:e5eb942643dc402fa1b8bd7e172729c491e7a61fe09ec8a57c101c7c691d468f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:bda5901203dbee5c6d9bde01c481b33f6d562a6b3a85805dc0cfb6ba4664b859
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314780794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8eb7a7a64c18845f082ce61105c3eee2101f611716c161e9f15764aee49b10`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:54:57 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Thu, 04 May 2023 14:54:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 14:54:59 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 04 May 2023 14:54:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 04 May 2023 14:54:59 GMT
WORKDIR /tmp
# Thu, 04 May 2023 14:55:07 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 04 May 2023 14:55:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 May 2023 14:55:07 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 04 May 2023 14:55:24 GMT
RUN boot
# Thu, 04 May 2023 14:55:25 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cf5ecc63589948ba9028f7a7ba75093cb9a0b0ec0aa545ceb047392800d2b1`  
		Last Modified: Thu, 04 May 2023 15:06:11 GMT  
		Size: 198.5 MB (198549481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4f2a1284601b5adbade366a1ae48e2fd63cffe9c2366de948b31a1fed3bfa8`  
		Last Modified: Thu, 04 May 2023 15:05:57 GMT  
		Size: 2.4 MB (2361723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcba720d446e207a4abd96e0875d7e9c2a019d5a7acd3bac7ce9bde7c24383d`  
		Last Modified: Thu, 04 May 2023 15:06:01 GMT  
		Size: 58.8 MB (58820520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f17a879ddf55c28fdf09b719cd8d2b7f1ebe6aeafab213ea1d0199498862f572
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.2 MB (310188429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef370a43f84214e1ff1a10fd8827d0afcd029ecd2d1756475684f19f9ccc588`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:26:55 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Tue, 23 May 2023 01:27:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:27:00 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 23 May 2023 01:27:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:27:00 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:27:04 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 23 May 2023 01:27:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:27:05 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 23 May 2023 01:27:23 GMT
RUN boot
# Tue, 23 May 2023 01:27:23 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e206de1cfcbe93e5295be6e8b68ac1878120e16eb1f6a6d4211f2d2a345f1fe`  
		Last Modified: Tue, 23 May 2023 01:35:30 GMT  
		Size: 195.3 MB (195324210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804226f8c0375eeda1223ccc8ba8c20433f8585e49ab0576f87fc575cee89474`  
		Last Modified: Tue, 23 May 2023 01:35:20 GMT  
		Size: 2.4 MB (2351050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6624e836eb681038457c128adac001b0b12465dc7599add77b50d2293d1d5576`  
		Last Modified: Tue, 23 May 2023 01:35:22 GMT  
		Size: 58.8 MB (58820557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
