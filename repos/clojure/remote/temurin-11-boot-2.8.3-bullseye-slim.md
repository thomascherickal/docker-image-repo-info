## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:761ce0f4629f35352a6ace57a05bceb06722c0e5f4e81c294b8cd1be94f2fb19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a483d754e6a21f829771e96bc5c79be20eef51114fe4bbf389b6b8c3fd76369c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289784831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e42235d2612d15ce3d48139b898de9a97236ebb25d38a1da4e8d14a1a3c4acb7`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:25:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:25:38 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:25:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:25:39 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:25:44 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:25:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:25:44 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:26:02 GMT
RUN boot
# Thu, 09 Feb 2023 09:26:02 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c3a4395db6d064c335f9de1395fc109ddf4084277fd1b33b28c3b0632b723`  
		Last Modified: Thu, 09 Feb 2023 09:38:35 GMT  
		Size: 1.1 MB (1077352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e37f7a4656365d767f2c5a778d2eaf5c65fd7fe86fdbddeb1f05884112f717`  
		Last Modified: Thu, 09 Feb 2023 09:38:38 GMT  
		Size: 58.8 MB (58820246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ae55c004de542202b2724a11233581b541c78f57fd7dd2293d45cf1f1e30e677
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285187946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e136389c2c8f9aa77d1bbb829d0cc0a4cec73649d3b72870e3a29fbf3c0b8220`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:21:30 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:21:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:21:34 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:21:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:21:34 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:21:39 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:21:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:21:39 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:21:54 GMT
RUN boot
# Thu, 09 Feb 2023 09:21:54 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf483a916e651ca447c4add0da489b56284ef3ab648f7c4b8b28762f912a1e`  
		Last Modified: Thu, 09 Feb 2023 09:32:44 GMT  
		Size: 195.2 MB (195240411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d11d295488b1c60cc4c84e8e41a835fd4c66d85e9301c4cc4b36fee374ba7`  
		Last Modified: Thu, 09 Feb 2023 09:32:33 GMT  
		Size: 1.1 MB (1064619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3954021db1fe82773f35577453ee47bf1a52ecc003475c5846f2fb6711f97cf7`  
		Last Modified: Thu, 09 Feb 2023 09:32:36 GMT  
		Size: 58.8 MB (58820407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
