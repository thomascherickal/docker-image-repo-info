## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:fa48e87c0a91fb4ffdb9cdeb5b836a524d06146906fea3d68e32e6f36f490332
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:325048217daf075536bbf9797ebf3b7da5f9bdf8b3a1f4bcf9df3ffa1f25677a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314678377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10542824e7295fb62988a78626c6ee46a409e4f969311b5e695232fc9531323f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:17 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:36:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:36:19 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 06:36:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 06:36:19 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:36:26 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 06:36:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 06:36:27 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 06:36:45 GMT
RUN boot
# Fri, 09 Dec 2022 06:36:45 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561532e76f8a67e2ac0114bf68c5fcb2c640ceb1eff7b0f331d366e73f673768`  
		Last Modified: Fri, 09 Dec 2022 06:53:29 GMT  
		Size: 198.5 MB (198454561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec4feadbcf8857579a8a61a13d86d360861febbbd417246d264d31db889a315`  
		Last Modified: Fri, 09 Dec 2022 06:53:15 GMT  
		Size: 2.4 MB (2362058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0ca3953739672ddd7763ec31a82b58018efb65a0d623e031e5d56d835542`  
		Last Modified: Fri, 09 Dec 2022 06:53:18 GMT  
		Size: 58.8 MB (58820416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:3bdbe312d9116a10153df30f0e6c99f4e3aaf99042dd77319be56306fdcc9ca1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310075334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f507ef80166a28e856fc45420f35a915f760e77de0c0f382b81ca0b13420af`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:03:32 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:03:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 05:03:36 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 05:03:36 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 05:03:36 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:03:42 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 05:03:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 05:03:42 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 05:04:00 GMT
RUN boot
# Fri, 09 Dec 2022 05:04:00 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1dc93c936f130a0b32765e5801ad37ff3679f9461520ae91ce9b6fa4d65888`  
		Last Modified: Fri, 09 Dec 2022 05:18:13 GMT  
		Size: 195.2 MB (195203416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e219abf9fbea314537b995be27f2a4efc9a3d2cf850832fc4947aa9dd118af0`  
		Last Modified: Fri, 09 Dec 2022 05:18:02 GMT  
		Size: 2.4 MB (2352310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be250b89bf6b3fb89b52f7b2c55af8056e8ac0491e4cae409df0f8018619f1f1`  
		Last Modified: Fri, 09 Dec 2022 05:18:04 GMT  
		Size: 58.8 MB (58820462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
