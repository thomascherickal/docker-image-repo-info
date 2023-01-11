## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:d52737fde085c5f7dea11de5945ad0e417f32fe5424df471f0d82e92c3f0a0c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:f0b5f84eebb7e0bc811afb2e4bd8d3f9878587c22438c09d7980f55074d80b1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.7 MB (289749333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11e420ef85380e13d7b22e499f2c270f7968c3e95298684ce3e4ba698e09a770`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:23:09 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:23:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:23:11 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:23:11 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:23:12 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:23:17 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:23:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:23:17 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:23:36 GMT
RUN boot
# Wed, 11 Jan 2023 03:23:37 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6154d41a3f1328e19471ffc2c51bb92391c00f8d743c0e0d90ec13704d92355f`  
		Last Modified: Wed, 11 Jan 2023 03:36:43 GMT  
		Size: 198.5 MB (198454554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8aacbdc703fb8bffb366db7bad141878085908a64edbb70ddec167ec5a1a1c`  
		Last Modified: Wed, 11 Jan 2023 03:36:28 GMT  
		Size: 1.1 MB (1077331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bceaf651a1403e224031700cb4daec4ed1daf0c5305a61ad234a31fca269ab`  
		Last Modified: Wed, 11 Jan 2023 03:36:31 GMT  
		Size: 58.8 MB (58820476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:dba1cd9380ff1a83bef0de8d82407ad3daad3b7c0affb6d59ecd0991aa52a3a8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.1 MB (285133570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239b4747966b535bb8ce852352a2326c8bfa7e0483b638ff119218c7d03c5273`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:41:23 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:41:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:41:28 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:41:28 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:41:28 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:41:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:41:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:41:33 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:41:51 GMT
RUN boot
# Wed, 11 Jan 2023 03:41:51 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b36725901023c32b079908ac189f7af623d07d41cf568b06bb3bc24cee19a2`  
		Last Modified: Wed, 11 Jan 2023 03:52:52 GMT  
		Size: 195.2 MB (195203408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7de7dfe2d7b84ed1eb922969cba3cb343a294258f5ba84425ee07abdb2c4c1`  
		Last Modified: Wed, 11 Jan 2023 03:52:40 GMT  
		Size: 1.1 MB (1064712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c14db79081f9002d7c902da5b7b062a299b2066c2867a6d206d742717fa17b0`  
		Last Modified: Wed, 11 Jan 2023 03:52:43 GMT  
		Size: 58.8 MB (58820636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
