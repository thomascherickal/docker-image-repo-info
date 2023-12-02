## `clojure:temurin-11-boot-2.8.3-bookworm`

```console
$ docker pull clojure@sha256:a4cbc53fc965586bd866958de9fac1a71be41a86eab7c8848560ef372ddd9014
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bookworm` - linux; amd64

```console
$ docker pull clojure@sha256:d825f8da6938824f341ceac89f9e3f3e302dd4a76c1a9134ea097968f747ec8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259199586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f059ad89fe5fb4f48f4f3ba99b7193ea0bda749a08f7c1c457447a329bf59d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:07:35 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:13:41 GMT
COPY dir:a96babc4beed1ce86268c08da8bb1232eedf77a64576d0e7cc109ca29beb78ef in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:13:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:13:42 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 21 Nov 2023 10:13:42 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 21 Nov 2023 10:13:42 GMT
WORKDIR /tmp
# Tue, 21 Nov 2023 10:13:48 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 21 Nov 2023 10:13:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 21 Nov 2023 10:13:48 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 21 Nov 2023 10:14:05 GMT
RUN boot
# Tue, 21 Nov 2023 10:14:05 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9e2ffce8b869cca4ab630c3d07ac20aef995e43238cf9b53a85805a1ce76cc`  
		Last Modified: Tue, 21 Nov 2023 10:31:55 GMT  
		Size: 145.3 MB (145266641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d98e033318ecb0baecd3faa24d8b948b073ed25b073b0cf5a4d1fb70542671`  
		Last Modified: Tue, 21 Nov 2023 10:31:44 GMT  
		Size: 5.5 MB (5530327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d35d76f3452a87f197aa1299d96ceb59d008e404e58e92ebdee35fae602a926`  
		Last Modified: Tue, 21 Nov 2023 10:31:47 GMT  
		Size: 58.8 MB (58820393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bookworm` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d2d454c07c8d306c0612ad8a0d45b284058abbfefbb232ae3e49c54317138468
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.8 MB (255788241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a669c089043090ef890ff163cf34087aae95d8c495eb1a36858f6a0142221ba`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:20:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:44:30 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 08:44:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:44:33 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Dec 2023 08:44:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Dec 2023 08:44:34 GMT
WORKDIR /tmp
# Sat, 02 Dec 2023 08:44:40 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Dec 2023 08:44:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Dec 2023 08:44:40 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Dec 2023 08:44:57 GMT
RUN boot
# Sat, 02 Dec 2023 08:44:57 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315e261122e4eab35c627bf04f6ca13cb4652c256e98fcc558b03f00b879462f`  
		Last Modified: Sat, 02 Dec 2023 09:03:38 GMT  
		Size: 142.0 MB (142001821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d22cd860770e2bb643fe5d797abf72bf3c74b192dd017c5592871165c9cbb05`  
		Last Modified: Sat, 02 Dec 2023 09:03:29 GMT  
		Size: 5.4 MB (5353236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab7f99c9346a39c0b9209d3ec93a6895efa0c2309ecbb7da5a9191b95a6c88d`  
		Last Modified: Sat, 02 Dec 2023 09:03:32 GMT  
		Size: 58.8 MB (58820534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
