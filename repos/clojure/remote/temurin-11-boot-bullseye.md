## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:610fdbed39226450d31e27ce6ae1afc3fa1abd7657f3fedb51ecf5db15927cbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:026ef70cd1ab7bea3bd8e2788e2e57df1a94df0802e7fcdcc6577d2bf40e95b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314787433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17bbbb8b973dfea5aecea85404d16c6e46fa93d92e3a3555f789490bb3113b45`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:46:56 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:46:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:46:57 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:46:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:46:58 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:47:03 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:47:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:47:03 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:47:23 GMT
RUN boot
# Tue, 13 Jun 2023 03:47:23 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12b8c3d504afe22ba8eb61403c46f5cc24b3d13561e5bdd23c0feed04b5a618`  
		Last Modified: Tue, 13 Jun 2023 03:57:02 GMT  
		Size: 198.5 MB (198549757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469c62e203ad725f6718a3cfbb7d7aa9551693af7dc52b415fb327da67663754`  
		Last Modified: Tue, 13 Jun 2023 03:56:48 GMT  
		Size: 2.4 MB (2362063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8212518e31e30a33dc2aff96b24baf7797e97bca491e7ca9e8a88acba229fe3`  
		Last Modified: Tue, 13 Jun 2023 03:56:51 GMT  
		Size: 58.8 MB (58820451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9684d92879661dafbf14201dc52387c7d9213db7e38e990c874dcfdafbd9ee41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.2 MB (310188839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e48db6cc8e5fad8c325b35efc997af0f660a1f4cc14d989f873ffe291fb74670`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Jun 2023 01:14:55 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Fri, 02 Jun 2023 01:14:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 01:14:59 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 02 Jun 2023 01:14:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 02 Jun 2023 01:14:59 GMT
WORKDIR /tmp
# Fri, 02 Jun 2023 01:15:07 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 02 Jun 2023 01:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 02 Jun 2023 01:15:07 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 02 Jun 2023 01:15:26 GMT
RUN boot
# Fri, 02 Jun 2023 01:15:26 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10120da7ed1ed5a24c9b69c8e805daf6a8b4d4752ac5ca258e31f04763958f`  
		Last Modified: Fri, 02 Jun 2023 01:24:39 GMT  
		Size: 195.3 MB (195324244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f028ffc26d33a0a57bc4ce62d558dc79846a13731c51f17c9d8e66452e5f437`  
		Last Modified: Fri, 02 Jun 2023 01:24:28 GMT  
		Size: 2.4 MB (2351361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b6217cd0c93cc46dd4761c8fa4bf1f8480b05fbbe6a9a3229bf500dee8dae7`  
		Last Modified: Fri, 02 Jun 2023 01:24:31 GMT  
		Size: 58.8 MB (58820622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
