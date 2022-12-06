## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:1c7e890440d8e50686f138412d5087cbd2fc29a35c9d79272f73b1d9a2d1c5be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:ec73fad6aaf0cb41adb2876a1c25129c62911ef9228694818e2203b8d648f603
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289767976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:139b42d978f09818ba8114aa5281aebfa1424637af03b48b1463b6ecdebd5480`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:52:17 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:52:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:52:19 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:52:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:52:19 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:52:25 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:52:25 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:52:43 GMT
RUN boot
# Tue, 06 Dec 2022 01:52:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b51844deb1462039b2a177cafb5f003ef0f5694191fab5310135e3307f2d3f`  
		Last Modified: Tue, 06 Dec 2022 02:05:31 GMT  
		Size: 198.5 MB (198455846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf1268fb3ad11383e468caf3207da04d153ca1c37ce84ddf58fc9b39563bcd`  
		Last Modified: Tue, 06 Dec 2022 02:05:17 GMT  
		Size: 1.1 MB (1078963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42674952a85fd426b570414871bb31666fa3ee73faec74074960d629467c6f7a`  
		Last Modified: Tue, 06 Dec 2022 02:05:20 GMT  
		Size: 58.8 MB (58820315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:7806b1000e117467ef37f3ada444c833d4c49dbf9aa2edca6c27f0ed30413fd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.1 MB (285148596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85848e7b1ece374ef8c43a68e7e54f128f0b9e15e4080a0b8c1bb913a03c7ffa`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:49:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 15 Nov 2022 05:51:59 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Tue, 15 Nov 2022 05:52:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 05:52:04 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 15 Nov 2022 05:52:04 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 15 Nov 2022 05:52:04 GMT
WORKDIR /tmp
# Tue, 15 Nov 2022 05:52:08 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 15 Nov 2022 05:52:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 15 Nov 2022 05:52:08 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 15 Nov 2022 05:52:26 GMT
RUN boot
# Tue, 15 Nov 2022 05:52:26 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cde71cdd6ac565f043bc4ec8903ab809981c13bc3c9e55dd5b7290a1bb0801`  
		Last Modified: Tue, 15 Nov 2022 06:03:30 GMT  
		Size: 195.2 MB (195201143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca3e675ac3bcfefb13e5fddac98a1a8446aae135c4d4df761f78af5a552c9b1`  
		Last Modified: Tue, 15 Nov 2022 06:03:19 GMT  
		Size: 1.1 MB (1066312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d86afbd018281c8beebe8a01f262ccdbc90e73c267fdfda166fad1fb672a616`  
		Last Modified: Tue, 15 Nov 2022 06:03:21 GMT  
		Size: 58.8 MB (58820536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
