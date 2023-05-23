## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:89fb61b65107e0711ea6eb448a40c195858b7cc4ef444a60e2c6db20fdd4c063
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b89d33a8ddd6a8acc122c28bf978a296afd522ac90c3f22e178d07d3d9189b1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289850923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273c82363e69c15527d96aa40124dec4c19156e877e0052d691ce9bd39bfbdeb`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:55:29 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Thu, 04 May 2023 14:55:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 14:55:31 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 04 May 2023 14:55:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 04 May 2023 14:55:31 GMT
WORKDIR /tmp
# Thu, 04 May 2023 14:55:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 04 May 2023 14:55:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 04 May 2023 14:55:37 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 04 May 2023 14:55:54 GMT
RUN boot
# Thu, 04 May 2023 14:55:55 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8debf5f3c7bd7d820f2797f8d4cfc95b7902d0071ca115228b3f6eb2d872a`  
		Last Modified: Thu, 04 May 2023 15:06:32 GMT  
		Size: 198.5 MB (198549506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e382d71c808d820f5da0501ec4fe06fb966f394c772c587f25a50d25834079`  
		Last Modified: Thu, 04 May 2023 15:06:19 GMT  
		Size: 1.1 MB (1077516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e5d393f3c2ba6bc94731cc572b7429f31b2b9adc99b5676e7e3759bb879f4`  
		Last Modified: Thu, 04 May 2023 15:06:22 GMT  
		Size: 58.8 MB (58820385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:047b99d79566924bc759c6d7694c8acf2842a2459cded89483d99159c3c3c281
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285262113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2df59acb56504e7cfb527662d196226e47c0838d31b2c9f812df402620013d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:27:27 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Tue, 23 May 2023 01:27:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:27:31 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 23 May 2023 01:27:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:27:32 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:27:36 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 23 May 2023 01:27:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:27:36 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 23 May 2023 01:27:54 GMT
RUN boot
# Tue, 23 May 2023 01:27:54 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78c86840ae584aab4d9f49c5158125ceb03a9fcfcbb243c03ce4819b42d8729`  
		Last Modified: Tue, 23 May 2023 01:35:49 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8689ac3ce4d3c0598666d82792f711aa16310029663a789710c67aa4ea280add`  
		Last Modified: Tue, 23 May 2023 01:35:39 GMT  
		Size: 1.1 MB (1064833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c183e2d37352ca85f0fa19e69f22d060717914ea55e5f280d7f1a43466e6716`  
		Last Modified: Tue, 23 May 2023 01:35:41 GMT  
		Size: 58.8 MB (58820324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
