## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:18656d85dc29227f0724dec182156071360d4314c0b28b15aac7b4371ff01a50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:675f39591a3b87dca8713d837862c83fe004ee5f593d2138d95085692770b071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145943662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1887ed3192248123f2dbda46e5478cdc4f857da4521d4bb4d933c3d494b2c3df`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:24:44 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Wed, 03 May 2023 20:24:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 20:24:44 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 03 May 2023 20:24:44 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 03 May 2023 20:24:44 GMT
WORKDIR /tmp
# Wed, 03 May 2023 20:24:50 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 03 May 2023 20:24:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 03 May 2023 20:24:50 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 03 May 2023 20:25:08 GMT
RUN boot
# Wed, 03 May 2023 20:25:08 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eda8d8deb246b934d051ef2af038ab3fb22f3de2f341e84edf173a887c496ab`  
		Last Modified: Wed, 03 May 2023 20:35:17 GMT  
		Size: 54.6 MB (54642103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba43ffca2c24151502031f77677dcd6464be46db2b2d635a5330f41436337a37`  
		Last Modified: Wed, 03 May 2023 20:35:11 GMT  
		Size: 1.1 MB (1077523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a103e70675e060920fe833f104b39d7480320577d31776adb431f58404e5fe1`  
		Last Modified: Wed, 03 May 2023 20:35:15 GMT  
		Size: 58.8 MB (58820520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d14e8ffeaeb1eba06e649c85e4f87ad46b8ea049bccdc301f88304eb5d431717
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143680689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd39a501698063d59cb9226721e141771e4011837a5533446272b70c93acc32`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:24:58 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Tue, 23 May 2023 01:24:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:24:59 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 23 May 2023 01:24:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:24:59 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:25:04 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 23 May 2023 01:25:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:25:04 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 23 May 2023 01:25:22 GMT
RUN boot
# Tue, 23 May 2023 01:25:23 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8239c1c9100b6b1e25d2af5517c297ca525746d0a3846be0e0c4fafd82271c3a`  
		Last Modified: Tue, 23 May 2023 01:34:17 GMT  
		Size: 53.7 MB (53742684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58543b7cac91943a9d4c3deaf1e2f41a3714d271e5bf8eaec92899061388e8a7`  
		Last Modified: Tue, 23 May 2023 01:34:12 GMT  
		Size: 1.1 MB (1064821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41fe02db6e84886a37c5fc77d3634a3fa719e3556351917247cf5fb69a41a3f`  
		Last Modified: Tue, 23 May 2023 01:34:14 GMT  
		Size: 58.8 MB (58820437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
