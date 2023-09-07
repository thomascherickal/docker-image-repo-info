## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:5bed7b9909cf88130003f60c899981683a5a4e866604cf98271750872df022d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:d1d61fd37a649d3cda02a8ca50d3508c093cef8c3517603576bf4073e0fe906d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236141633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a6ff7a5385f749d4b347376d4cf3791823605b385eb2e9e83d42dcfecfd6ed`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:03:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 02:04:50 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Thu, 07 Sep 2023 03:21:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 03:21:27 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 03:21:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 03:21:27 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 03:21:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 03:21:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 03:21:33 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 03:21:52 GMT
RUN boot
# Thu, 07 Sep 2023 03:21:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc2204a29ef2517e9d39b89552fcfbd45063a2d758626e1aef118a701134c2d`  
		Last Modified: Thu, 07 Sep 2023 02:07:35 GMT  
		Size: 144.8 MB (144826055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bb3fc1e9accf2b4c731f8192c44372f9f3948737a1cd2d069d477c725d4426`  
		Last Modified: Thu, 07 Sep 2023 03:31:33 GMT  
		Size: 1.1 MB (1077548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b12b1ef07ecbb22e7c859f3c98ecfa1ec57a96d529e31b9be42def5fef40602`  
		Last Modified: Thu, 07 Sep 2023 03:31:36 GMT  
		Size: 58.8 MB (58820527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:999acd17216707036a473ffbbd2a1845b8fdd5a5bac8d4fa6179b9c0a73a489a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231518520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f2059fed78f5cfe86284e01b26f220946ccb67fd589c9a8eeb2b0d29b18b0`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 07 Sep 2023 06:47:24 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Thu, 07 Sep 2023 09:07:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 09:07:09 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 07 Sep 2023 09:07:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 07 Sep 2023 09:07:09 GMT
WORKDIR /tmp
# Thu, 07 Sep 2023 09:07:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 07 Sep 2023 09:07:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 07 Sep 2023 09:07:14 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 07 Sep 2023 09:07:32 GMT
RUN boot
# Thu, 07 Sep 2023 09:07:32 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b018ed6a392610f1ab69e85cc642842b49d22521199586d6067dfd326f17f2`  
		Last Modified: Thu, 07 Sep 2023 06:49:54 GMT  
		Size: 141.6 MB (141570382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1b02bec70918e3ed138026de64cfaff1608af9031a657fbb661b095238b03a`  
		Last Modified: Thu, 07 Sep 2023 09:16:12 GMT  
		Size: 1.1 MB (1064804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea4d7e18efa87880c0d0797cbbe61f3dc242d0897dcfb467b9505957310b5d8`  
		Last Modified: Thu, 07 Sep 2023 09:16:15 GMT  
		Size: 58.8 MB (58820431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
