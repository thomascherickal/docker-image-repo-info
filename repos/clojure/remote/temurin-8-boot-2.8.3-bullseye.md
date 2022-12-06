## `clojure:temurin-8-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:49d017f5539b7e0ca3694ba0ac29c8076120701a1b7b05dc2395545779b63e98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b3eff50ab38b3fb6cee12d7a356969b8f51d3094032af510571e0cedf60c917e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.8 MB (219754544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c076581cca0c7248c7d27462e2d57d90764d1b1a8515bd49634929fa7ade2a16`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:48:45 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:48:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:48:46 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:48:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:48:46 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:48:53 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:48:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:48:53 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:49:14 GMT
RUN boot
# Tue, 06 Dec 2022 01:49:14 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d55e2e180666cd09635874932249e6b38c8a236bbe474c85aeeaf3a3e9c48c2`  
		Last Modified: Tue, 06 Dec 2022 02:03:18 GMT  
		Size: 103.5 MB (103530693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b28b6ab12e08b8e0a55e96f3bd7820b34a5771e305e011d8073a2a20eb2f7`  
		Last Modified: Tue, 06 Dec 2022 02:03:09 GMT  
		Size: 2.4 MB (2362026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7da9638b34aa0ed8b83f8b306bdfe7d7682fd2d94fb21f29d5644d2b1f6bc08`  
		Last Modified: Tue, 06 Dec 2022 02:03:12 GMT  
		Size: 58.8 MB (58820483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f2cf06cc407bb9fcfd8314ec3f6a4941609b73db02c7ee53d6063132c106256f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217498537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f91966b2ae2281787ab1df0fff843d2e3d3a7a6d1caec282ec93bb27dd91071`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:17:16 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:17:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:17:19 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:17:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:17:19 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:17:24 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:17:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:17:24 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:17:42 GMT
RUN boot
# Tue, 06 Dec 2022 02:17:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f371d9828c94870641f3c611f4a9fda6d693a78baa752a2efcea3cab5826d80`  
		Last Modified: Tue, 06 Dec 2022 02:29:56 GMT  
		Size: 102.6 MB (102626604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c9a08001941fb9e97b97c3964f824664edc02713a8b27d3587ddada81b9579`  
		Last Modified: Tue, 06 Dec 2022 02:29:50 GMT  
		Size: 2.4 MB (2352251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5037a4334cd0e4c8098c604f58ce1009dc4e5064577bdfeebf3b00d0a778a3`  
		Last Modified: Tue, 06 Dec 2022 02:29:52 GMT  
		Size: 58.8 MB (58820536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
