## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:b512f0899d523641d36ef18a4d21a0f9e96f6dfa7ce7a2dba9f65bdb1ac5447f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

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

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5360fcc12f836c9922890cd7e7edb884ae1a73cefdd58e09b2b6024750fb6030
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.1 MB (285148267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:303ad6bfb7f41e07b8f49a812f01027295f40e416486757fb0a9ba41f507fa4d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:20:18 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:20:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:20:23 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:20:23 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:20:23 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:20:28 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:20:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:20:28 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:20:44 GMT
RUN boot
# Tue, 06 Dec 2022 02:20:45 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ee26ba69cd8afd37462741fda4929d6658730baa6af64ace9a30c2c6aa3b9`  
		Last Modified: Tue, 06 Dec 2022 02:31:55 GMT  
		Size: 195.2 MB (195201090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee14ab82b6ddb4d9e8aa29f93a2f1ffdd07c6a089c4e8ba69f459a16bbb4e78`  
		Last Modified: Tue, 06 Dec 2022 02:31:44 GMT  
		Size: 1.1 MB (1066346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaff9e20fa1eb36954b3e03c820289df02d8aa762105b70cdb460327d82813d2`  
		Last Modified: Tue, 06 Dec 2022 02:31:46 GMT  
		Size: 58.8 MB (58820511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
