## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:c41b574f68d5a882a3af39d1c5805edfffb970c7267db5188d7afb5e7cd92cf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:20566a0be5d359b284468a4f000bbea92e0fa3b7d85071d05f5b1fd33a8677de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314703715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b327c0077d26e8f4fc8722424bd3b79ee57cc1938e46bc8aab3705ba23b3ce`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:16:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:19:58 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:20:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:20:00 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:20:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:20:00 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:20:06 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:20:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:20:06 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:20:23 GMT
RUN boot
# Thu, 23 Mar 2023 06:20:23 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab656fe58b67db3e6051a8b99a09ffa77a9d8123326d18547c28803ea6e0439`  
		Last Modified: Thu, 23 Mar 2023 06:30:46 GMT  
		Size: 198.5 MB (198476073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9134c860de795517c920387f54f89973cd2cbff11b205254d1db12eac1784b4`  
		Last Modified: Thu, 23 Mar 2023 06:30:33 GMT  
		Size: 2.4 MB (2361568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea413de62dc105ccbfd7f7a8e07773f57769ccefc747f463b869d1e17be75c6`  
		Last Modified: Thu, 23 Mar 2023 06:30:35 GMT  
		Size: 58.8 MB (58820466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:85e2eb5aaf580c1c884165a39743cc5dc268d73768067da67eb12841b56c7a78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310117083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b40b356209ee944d74eb2f4386f6921caa625834d12359b45f701bdbc7fcfbf`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:54:29 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:54:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:54:33 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:54:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:54:33 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:54:38 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:54:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:54:38 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:54:55 GMT
RUN boot
# Thu, 23 Mar 2023 06:54:55 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdf724c79e8ef28b4558428377d3e80e17fbb6d9e7687eccd5e057f9148f334`  
		Last Modified: Thu, 23 Mar 2023 07:04:00 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbe77283187da630ed6202b9689d3148ca94683524f4a3531d9562020d02fee`  
		Last Modified: Thu, 23 Mar 2023 07:03:49 GMT  
		Size: 2.4 MB (2350958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5c805d96973106020f5e47b845ed07bd9e9f544bd8387be4254e0da6d737d0`  
		Last Modified: Thu, 23 Mar 2023 07:03:51 GMT  
		Size: 58.8 MB (58820519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
