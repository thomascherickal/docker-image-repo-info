## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:45d53a587a6d6d4b930623960aabf68abd1318b72a99ce3eb435e428c26fa979
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:dd2542227b6d3b2c7113281f3e5c72571ab34fbfbe769329f5124f9051d6f406
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314679597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad205a07462a8279c0e91768036f22c74c83de1adc88bbbca6a054292c18b8f5`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:51:45 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:51:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:51:47 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:51:47 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:51:47 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:51:52 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:51:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:51:53 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:52:11 GMT
RUN boot
# Tue, 06 Dec 2022 01:52:11 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c5438c0c2e12b199078d9f749cb1d284d54ba850653ab042ebcb6578bcd6ea`  
		Last Modified: Tue, 06 Dec 2022 02:05:07 GMT  
		Size: 198.5 MB (198455802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db69489a92b69c47dbe997806ea4235e77dba5c092569e0ef7d569f581003e43`  
		Last Modified: Tue, 06 Dec 2022 02:04:52 GMT  
		Size: 2.4 MB (2361966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a239b0604498b2566dc1f34e47b317cffbeef69f0a4b00fa9a2e794edb3d00`  
		Last Modified: Tue, 06 Dec 2022 02:04:55 GMT  
		Size: 58.8 MB (58820487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a8887e8aa383948485ef88a8856d3dba9e8f59ff54c1050f88dcb5ddd3ddf0c6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310072863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:467d29a64f69b5b113cef2b4ffd108c43d8f9128b45f7075b566d35f103c7879`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:19:46 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:19:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:19:50 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:19:50 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:19:50 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:19:55 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:19:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:19:55 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:20:12 GMT
RUN boot
# Tue, 06 Dec 2022 02:20:12 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e57d0f48cefee9792c2b89dfe1d1b4e7f06248afb63cf243b95a4cce821459`  
		Last Modified: Tue, 06 Dec 2022 02:31:35 GMT  
		Size: 195.2 MB (195201090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500811fb310babe388fefa2c64f14cfac1b0042d09a0c372a9a333f5bc37bdab`  
		Last Modified: Tue, 06 Dec 2022 02:31:20 GMT  
		Size: 2.4 MB (2352218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d884bf6687d1ca51474d9562772c95fa8dcb263f48e5b48ec89e808f557b0dbc`  
		Last Modified: Tue, 06 Dec 2022 02:31:23 GMT  
		Size: 58.8 MB (58820409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
