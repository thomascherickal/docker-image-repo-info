## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:77d5b685fd44e063b14d0874ac1e08ee2b978e7b9c0b028bfa4b3e199f28f5b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:12f610eba093803cd29027aabce96c545a7a377f29f86417e270aa84201df2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194825435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdd93c2d7f5a9bed19d7388a2ad2153e416a470255a2812a32b6edb98478632`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:20:06 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:20:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:20:07 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:20:07 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:20:07 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:20:13 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:20:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:20:13 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:20:33 GMT
RUN boot
# Wed, 11 Jan 2023 03:20:33 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ade43ff5ddf2dd9ad42891c3aa91290adf691b595fbeb5ae8f18f8f74edb57`  
		Last Modified: Wed, 11 Jan 2023 03:34:49 GMT  
		Size: 103.5 MB (103530647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38ffddfeec417842d274f1a1d2b1a9438b932993774bc2b9e99c4f35fa581cc`  
		Last Modified: Wed, 11 Jan 2023 03:34:40 GMT  
		Size: 1.1 MB (1077361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b388ab5c45635b2d24b330793ccd235544ae2a16412fcbfffbff75849348a`  
		Last Modified: Wed, 11 Jan 2023 03:34:44 GMT  
		Size: 58.8 MB (58820455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b78b045ba23e9af0f58a446420d658414620c239a4e358f35cb64a643194e485
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.6 MB (192556697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c95f386687d2eb45a25bdcf3887d22bcf6bc2f0ce8991177e7e6f53060d53fc`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:38:49 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:38:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:38:51 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:38:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:38:51 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:38:56 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:38:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:38:56 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:39:15 GMT
RUN boot
# Wed, 11 Jan 2023 03:39:15 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce85b39ca353502b73ca7a3525ce50c3eb8348c68963e1b5d5d21f28da7b8db1`  
		Last Modified: Wed, 11 Jan 2023 03:51:13 GMT  
		Size: 102.6 MB (102626602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e938c26fd17756606b6fdff8dc8eec8017a66686ca5e39e152a85ce2704286f6`  
		Last Modified: Wed, 11 Jan 2023 03:51:06 GMT  
		Size: 1.1 MB (1064701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3aec88731a4592fb281e4b36049267472f77ebf7b29943a20604fb19be1487`  
		Last Modified: Wed, 11 Jan 2023 03:51:08 GMT  
		Size: 58.8 MB (58820580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
