## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:80f11dbda5587f1516e9ca29019de94253df4b62c7ab3a2ca281858bd86f95ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:e6869a5fd70eb40cd84e7f378c2ee10063d455d9aec4106d1e2bdc3ce83090ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145945059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071404a1e7b371d40da4a8c0fe6e8a1a47d5e7871fb96ae21bbf40f496269279`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:22:39 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:22:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:22:39 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:22:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:22:40 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:22:45 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:22:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:22:45 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:23:03 GMT
RUN boot
# Thu, 09 Feb 2023 09:23:03 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff09d33db7932dfdb13e1ebfdd9d02620a26713de0236d8aef1f5d2e115b133`  
		Last Modified: Thu, 09 Feb 2023 09:36:59 GMT  
		Size: 54.6 MB (54635563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0d2df04ebc3f16cfa2fdfd3b38c2cc57f43e096aa636ca6890150d6ee862df`  
		Last Modified: Thu, 09 Feb 2023 09:36:52 GMT  
		Size: 1.1 MB (1077361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3226138d3d8ae22581284220c2ab32e76f9d06c04f982ff80d98ede98c3e421`  
		Last Modified: Thu, 09 Feb 2023 09:36:56 GMT  
		Size: 58.8 MB (58820325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:15dd46ace1e6a9ad54cf92cc8516050b9a6e39831e5ed0108d991cb956aba26a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143675309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a890ddb50a221bf1122c50e45e48e77ecc2266698c3288a241c0db3ecdc03946`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:18:59 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:19:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:19:01 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:19:01 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:19:01 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:19:06 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:19:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:19:06 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:19:22 GMT
RUN boot
# Thu, 09 Feb 2023 09:19:22 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd68f0bab68b42136c4251287a12f055f74853a5f1d694a98637f9f09e4ed94`  
		Last Modified: Thu, 09 Feb 2023 09:31:02 GMT  
		Size: 53.7 MB (53727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c52c6694b09825b40d08d4a0051915c2fa9e7c52e2ee614642321955694ae`  
		Last Modified: Thu, 09 Feb 2023 09:30:57 GMT  
		Size: 1.1 MB (1064593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1361d1a392eee325f9b45fd812e68ae853061522076a2c127ca85fa0dafbd531`  
		Last Modified: Thu, 09 Feb 2023 09:31:00 GMT  
		Size: 58.8 MB (58820288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
