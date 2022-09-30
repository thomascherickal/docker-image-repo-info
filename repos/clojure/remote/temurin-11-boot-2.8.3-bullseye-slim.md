## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:13260fd206fc9eac4078731f328ba371b3eb6660c0fb60c47e77f4cb392d9913
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:123de99a0c3fc5e76ab8b3eff1974dd7b317054810c289ab53ca42562d81f45e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.4 MB (289427112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9519b38c33c315ad2738873bdc1f18653963225dfba83a7e8d2d78a66e7a51b4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Sep 2022 06:18:45 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:24:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:24:40 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:24:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:24:40 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:24:46 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:24:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:24:46 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:25:11 GMT
RUN boot
# Fri, 30 Sep 2022 22:25:11 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a2774ad4f184f0a10c74dd66c9b4fdf76a60a8dbb311b9499b3173aabfcc61`  
		Last Modified: Tue, 13 Sep 2022 06:24:44 GMT  
		Size: 198.1 MB (198124887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430a2a2ef6ab4a7752bbe178ba2a51bbf44b7e73b3c998ca2f011589c187a19`  
		Last Modified: Fri, 30 Sep 2022 22:37:48 GMT  
		Size: 1.1 MB (1077322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f224d53b9a94a9f35a8847687b107bee4a3083dffb0442c826dd192fa6cf1152`  
		Last Modified: Fri, 30 Sep 2022 22:37:52 GMT  
		Size: 58.8 MB (58820782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:fa595bc53f30730e871bf78248b2066608d43e5b79fe60de0fffadec7467f94a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.8 MB (284801965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d5508b29752c6bba83ba8fc293117912d39793d8ac780f7d04630413b238ff`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Sep 2022 06:58:16 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:44:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:44:51 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:44:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:44:53 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:44:59 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:45:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:45:01 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:45:15 GMT
RUN boot
# Fri, 30 Sep 2022 22:45:16 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4184f46e59fa544d67090bc1b94d36f2af8c4757717aecdc90e0819aadac9`  
		Last Modified: Tue, 13 Sep 2022 07:01:59 GMT  
		Size: 194.9 MB (194867856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd97ce0de4f406388abeecc101deb3d0dc29486c92bbd8454d5fbd160ab0fa`  
		Last Modified: Fri, 30 Sep 2022 23:02:47 GMT  
		Size: 1.1 MB (1064290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc1e70ac242be99b2d19f717b64b1fe3fcb5343b5307e72649cdc4dd50fc9a0`  
		Last Modified: Fri, 30 Sep 2022 23:02:52 GMT  
		Size: 58.8 MB (58815580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
