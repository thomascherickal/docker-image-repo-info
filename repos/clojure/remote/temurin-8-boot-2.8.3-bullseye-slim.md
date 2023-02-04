## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:589d50c3de34cc671ae177dd5bec41fe13656a29de14c36723ed8f1ed4e6cb20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:0a5ace97f73b34fcd5e3c8f34e4fa0824b3a40ff28614dd84c8d5df9bf325853
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145930176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:318a3d3464af595620c2e5f2ce32ff7bf61526101881144573af7f6263ac37ff`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:06:08 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:06:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:06:09 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 04 Feb 2023 14:06:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 04 Feb 2023 14:06:09 GMT
WORKDIR /tmp
# Sat, 04 Feb 2023 14:06:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 04 Feb 2023 14:06:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Feb 2023 14:06:15 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 04 Feb 2023 14:06:32 GMT
RUN boot
# Sat, 04 Feb 2023 14:06:33 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2e51264c882c87c91946d030677c2c91c91959e652ff8ca78e35a61148bb39`  
		Last Modified: Sat, 04 Feb 2023 14:20:17 GMT  
		Size: 54.6 MB (54635589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c067a30284dd788e8e808a4fa7c646e6044b0de6df884ed6180fa204f735b`  
		Last Modified: Sat, 04 Feb 2023 14:20:10 GMT  
		Size: 1.1 MB (1077364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6260cb86b965d87680bec50fcfea6906c23783231e0b09fa3f322c09b574d29`  
		Last Modified: Sat, 04 Feb 2023 14:20:13 GMT  
		Size: 58.8 MB (58820304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:dd08e34c66a339365f7a1160f1f4615beeb875b10c009d7582541ba62d89b298
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143657653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7b35511bf57e46d6bd3e9952f043a871af8396d81a3949504af1c6daabeaf3`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 20:00:58 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Wed, 25 Jan 2023 20:01:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 20:01:00 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 25 Jan 2023 20:01:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 20:01:00 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 20:01:04 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 20:01:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 20:01:05 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 25 Jan 2023 20:01:21 GMT
RUN boot
# Wed, 25 Jan 2023 20:01:21 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007684b573bff2526d1b392ce3c4076e52d5a400dc5f5c38e5a8aa784c21bb07`  
		Last Modified: Wed, 25 Jan 2023 20:13:02 GMT  
		Size: 53.7 MB (53727884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0579228e55d19b24011588b6f0d85db2c9171d79dfe6f4cb4a4260f05cadfb`  
		Last Modified: Wed, 25 Jan 2023 20:12:57 GMT  
		Size: 1.1 MB (1064708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d0ec6d8813e6873710e6fd8cb65e8b9ff9ef102d341e61baf222c9b879819`  
		Last Modified: Wed, 25 Jan 2023 20:13:00 GMT  
		Size: 58.8 MB (58820247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
