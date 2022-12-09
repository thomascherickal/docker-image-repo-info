## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:fa097ed710e64d6ce0525171232a6a26be9490a63c5697d82aca6167f471d1b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b195749c811da507915621260c0197b8000427f0e36606c3c8f1cda01eefaf9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289766766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b05f5d68f3e672ffcf86695b087690355071573952c03d5a3a7cc0d6d09712`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:36:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:36:57 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 06:36:57 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 06:36:57 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:37:03 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 06:37:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 06:37:03 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 06:37:21 GMT
RUN boot
# Fri, 09 Dec 2022 06:37:22 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b513ff0d4a9663cc26bf2be1e84931ccd5a100516e08dc6c5d64ce16726a7fd`  
		Last Modified: Fri, 09 Dec 2022 06:53:38 GMT  
		Size: 1.1 MB (1078977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf09a42780debdd73f8cbf28b11deebb41d3d12551f7db9bff38fc06cc438f6`  
		Last Modified: Fri, 09 Dec 2022 06:53:42 GMT  
		Size: 58.8 MB (58820381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cfb4f3f115af53637430e180ab49c65967c2991d40265da43141db66414c1923
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285150545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75b64843c9a04faaa709cfc4d2444db7238946275436ffa59bdff1061a9d4cd4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:04:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 05:04:09 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 05:04:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 05:04:09 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:04:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 05:04:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 05:04:14 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 05:04:30 GMT
RUN boot
# Fri, 09 Dec 2022 05:04:30 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586a33c617d9a859a261455aac0fe9c9c611b0792c02b625cd8bffb638c7350e`  
		Last Modified: Fri, 09 Dec 2022 05:18:27 GMT  
		Size: 1.1 MB (1066319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c612765bf6d3af90e14436ba66ce0db6e66dcf38514c0a885037440b699c7b8d`  
		Last Modified: Fri, 09 Dec 2022 05:18:30 GMT  
		Size: 58.8 MB (58820534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
