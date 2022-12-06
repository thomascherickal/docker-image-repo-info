## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:e75e25e2386604f2239d35f8ebc35b572d494394e9bd6e109d0a4e8e6d6fdfbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:e18b30fbcd44559983ae2b7233b05b74453eb7d335aae81348b7c7b83ea360f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194842999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6c22f87cf2be44b9fb565b0c635c38b2f248b9456496a49034f7549d5610c80`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:49:18 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:49:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:49:19 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:49:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:49:19 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:49:25 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:49:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:49:25 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:49:44 GMT
RUN boot
# Tue, 06 Dec 2022 01:49:44 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4affc3cd73f667de2263e106409ed3d854f8bd2cd76ecd0a5e3aca312c862bff`  
		Last Modified: Tue, 06 Dec 2022 02:03:39 GMT  
		Size: 103.5 MB (103530647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6f8f20c0b9270f385fb45c9cd3f23ef453a0d82875c85f691e4f5dee33c920`  
		Last Modified: Tue, 06 Dec 2022 02:03:27 GMT  
		Size: 1.1 MB (1078974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ba78294ebf94ff385f3d683eca241d34f438e6b162372ec3cb3698875b54d`  
		Last Modified: Tue, 06 Dec 2022 02:03:30 GMT  
		Size: 58.8 MB (58820526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c83a665ea60027cd1ebee7e3aa997f1d256dd6c0e8c0dfbdeccb02571802e52f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.6 MB (192573651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5e0c64054782ea01f14d9439e49f2b36cab075e39e4e34d088424015361e916`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:17:49 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:17:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:17:52 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:17:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:17:52 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:17:56 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:17:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:17:57 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:18:15 GMT
RUN boot
# Tue, 06 Dec 2022 02:18:15 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5df8fef8a794006d98d0afa5f4cd031bef7bb0b991129e393fd59e5565be509`  
		Last Modified: Tue, 06 Dec 2022 02:30:13 GMT  
		Size: 102.6 MB (102626601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068360cd2a66102d4f509386cc60eab15a045b4c635d7d39041497c9aadbdf24`  
		Last Modified: Tue, 06 Dec 2022 02:30:06 GMT  
		Size: 1.1 MB (1066307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94e9157ff9c364cf004f3971692a06ac81ccbb6a3929b82b98237691c955d23`  
		Last Modified: Tue, 06 Dec 2022 02:30:09 GMT  
		Size: 58.8 MB (58820423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
