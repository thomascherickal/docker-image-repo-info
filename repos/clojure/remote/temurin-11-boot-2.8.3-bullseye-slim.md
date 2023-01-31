## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:8cbe6bb6480a58837285f62c1f1acce38470eb3922b7233adde8c2e6ff45c530
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:26848645623c20b92382c362b8cf8aaa442462336158a8030fddcfa721980a9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289770361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db1a538d9f17847404009af608f2124cb0ce8bd0b23a671cf45882a39ec3c69`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 00:39:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 00:39:30 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 25 Jan 2023 00:39:30 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 00:39:30 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:39:35 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 00:39:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 00:39:36 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 25 Jan 2023 00:39:53 GMT
RUN boot
# Wed, 25 Jan 2023 00:39:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0912d1d7c0ff2fea0c77f796175bc3b72c42d2365f964b9d77593f82095bc54`  
		Last Modified: Wed, 25 Jan 2023 00:54:18 GMT  
		Size: 1.1 MB (1077331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985c5da5b0630796dff5d213bd6a642875111b1105c91a6ce7f33e95afbaab22`  
		Last Modified: Wed, 25 Jan 2023 00:54:21 GMT  
		Size: 58.8 MB (58820352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8345d176b31933170ba4155143158dacf8d8a19b5cdd2ab6efd29f197c7d9c71
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285170253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e1a0e8ed0ea783714bf81011610059f12aaf0dea23f9889f0e8941cd416ab9`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 20:50:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:50:16 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 31 Jan 2023 20:50:16 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 31 Jan 2023 20:50:16 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:50:21 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 31 Jan 2023 20:50:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 31 Jan 2023 20:50:22 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 31 Jan 2023 20:50:40 GMT
RUN boot
# Tue, 31 Jan 2023 20:50:40 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e435c5f718cb8031f50e14c7fe179028adbc439627711fe2846fd44e7fe708`  
		Last Modified: Tue, 31 Jan 2023 21:04:22 GMT  
		Size: 1.1 MB (1064677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52058ee7835930862313ce34be594de169216362f1f45e4872cd7b3e5e3aa55`  
		Last Modified: Tue, 31 Jan 2023 21:04:25 GMT  
		Size: 58.8 MB (58820460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
