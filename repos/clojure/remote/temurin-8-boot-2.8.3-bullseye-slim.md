## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:527fd0f4a0be851d42f5c4e3f4a9592db71f97bca5281b4a1e0f4b82dbb09e81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:83c509b8fc6bed073eb3913795556a6ec511602acc31bc24599bec80dca2a31f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.0 MB (145957654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca2a236faf7560c8e084ac5417f09096528432fa4c60eaec4a144dbfeb3e0ed`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:44:38 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:44:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:44:38 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:44:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:44:38 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:44:44 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:44:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:44:44 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:45:04 GMT
RUN boot
# Tue, 13 Jun 2023 03:45:04 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a06b2482c1581bf48768b9037153a524f6626b4fdbab3333e123405ee98c4d`  
		Last Modified: Tue, 13 Jun 2023 03:55:36 GMT  
		Size: 54.6 MB (54642102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70be3158a98adeb47fc61efc83b7dcd346740355508515d5f8109db2e09a21`  
		Last Modified: Tue, 13 Jun 2023 03:55:30 GMT  
		Size: 1.1 MB (1077509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa0a26ad0b8d03d61ba1be2a97ecec908d8b71ebdbc54067d88b001876ceb61`  
		Last Modified: Tue, 13 Jun 2023 03:55:33 GMT  
		Size: 58.8 MB (58820633 bytes)  
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
