## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:f781db63136606f78b820439f16b33d63bcc776df7ed0ef018849281ba6283c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b826b517e5d7c9d36dac141d708e7dea5f0d160421bbdce2bfd100a6b3dbce2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289864844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea9185e35400532a55d3de9b642becc00b2a8261261edf6f86b78ecf5657005`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:00:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:19:30 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Wed, 05 Jul 2023 11:19:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 11:19:32 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 05 Jul 2023 11:19:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 05 Jul 2023 11:19:32 GMT
WORKDIR /tmp
# Wed, 05 Jul 2023 11:19:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 05 Jul 2023 11:19:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 05 Jul 2023 11:19:37 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 05 Jul 2023 11:19:55 GMT
RUN boot
# Wed, 05 Jul 2023 11:19:56 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099caecba99bf99b21cfbb7f1c23915fe48406202f54aa425cdb8d4341babebd`  
		Last Modified: Wed, 05 Jul 2023 11:32:56 GMT  
		Size: 198.5 MB (198549444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433fd9bcc0cf5238347c5e68dca7a3524729e24ffa19ae1aae946329d43d6bb3`  
		Last Modified: Wed, 05 Jul 2023 11:32:43 GMT  
		Size: 1.1 MB (1077515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708b6a13a082d7b3a43edc526df7ae92f0e32e81126b344f32aecad2652a4125`  
		Last Modified: Wed, 05 Jul 2023 11:32:46 GMT  
		Size: 58.8 MB (58820497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:efac4873ec679cb74fe878d1f65559a486e0163bf23b9fea3d52e5cf1f390e79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231513652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13642b4abde123b76e73f01d1a9924565731fd4929a2eb491e37d8e3eb95b8b9`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:34:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Jul 2023 01:07:37 GMT
COPY dir:e71da8247d58ed4b0dfbf219951c863c79ac94b7f45cb60320ea827dfa699275 in /opt/java/openjdk 
# Wed, 26 Jul 2023 01:07:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 01:07:41 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Jul 2023 01:07:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Jul 2023 01:07:41 GMT
WORKDIR /tmp
# Wed, 26 Jul 2023 01:07:46 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Jul 2023 01:07:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Jul 2023 01:07:46 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Jul 2023 01:08:04 GMT
RUN boot
# Wed, 26 Jul 2023 01:08:04 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9764bfc347c8d9f94a13dbe1948f4a4e50fef24a4e1e5730fab2710cb583db8`  
		Last Modified: Wed, 26 Jul 2023 01:13:46 GMT  
		Size: 141.6 MB (141565338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6117a15f62d8e4b6823604bc34a8d5b5810cb151a5f992622f7552f891c6b147`  
		Last Modified: Wed, 26 Jul 2023 01:13:37 GMT  
		Size: 1.1 MB (1064823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e4197f60cad0f7ea92bd1f54ef59922b81af0e68e468a4a5f31bdfa576bcc5`  
		Last Modified: Wed, 26 Jul 2023 01:13:39 GMT  
		Size: 58.8 MB (58820534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
