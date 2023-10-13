## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:b57375e8e8f029546cf72cfc1ac915ecbc778d1a4ca39783c588d5a0209cd806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:0fe630a1ed645f6748c43987d50cd79f876caae8fd91ec3173b3e010dda14514
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261073581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8dab46f6033ed243b2ab276e2c63fce2a862bc2b33c4524f5275d9923c867f9`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:51:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:45:01 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:45:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:45:02 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 13 Oct 2023 12:45:02 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 12:45:03 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:45:09 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 12:45:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 12:45:09 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 13 Oct 2023 12:45:27 GMT
RUN boot
# Fri, 13 Oct 2023 12:45:27 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb795fe3c9891f009fd979aba8b303ac17d8263f44bbed3ded94759592267537`  
		Last Modified: Fri, 13 Oct 2023 13:05:34 GMT  
		Size: 144.8 MB (144826232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc525c5d6277d1f3ca86e64ddce43c2087f3941a5d414f186220583e129af72`  
		Last Modified: Fri, 13 Oct 2023 13:05:23 GMT  
		Size: 2.4 MB (2368722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d014dc9fb1b7eeb21eba5d6449d5b4ba93bfd75a731f9e37a56eb842eb46299`  
		Last Modified: Fri, 13 Oct 2023 13:05:27 GMT  
		Size: 58.8 MB (58820599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6a2a589688d309f1dbe7532f3eb98ac3ee44c623506ac021a4fe047e56c06109
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.5 MB (256456147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50bd5ba429038377bfde01e02d0a41bd123c058f739158886efdb36d62b0e90a`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:45:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:13:03 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:13:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:13:06 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 13 Oct 2023 10:13:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 10:13:06 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:13:11 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 13 Oct 2023 10:13:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 10:13:12 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 13 Oct 2023 10:13:28 GMT
RUN boot
# Fri, 13 Oct 2023 10:13:28 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84f7633d1d2771c9ab00f2a01ba865738fa3a78d5441c5b21022c97aeaa5ebe`  
		Last Modified: Fri, 13 Oct 2023 10:30:01 GMT  
		Size: 141.6 MB (141570530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57121be3864645ea074d3427fa127a28e91bfde938c42f3d1eed2305ec869bf`  
		Last Modified: Fri, 13 Oct 2023 10:29:52 GMT  
		Size: 2.4 MB (2357439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4da1c22df7e0103986bf1d3cb2224cd64356f3a7ed5eae0ab37dcec35a730f8`  
		Last Modified: Fri, 13 Oct 2023 10:29:55 GMT  
		Size: 58.8 MB (58820368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
