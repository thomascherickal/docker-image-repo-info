## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:b4a53aeb5f45a7fe4ab87e99f4af48539bbd02473ac655e3b4a43c4d7a73e1af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:7b0444e99d18d2625a97e2aa5fb677d13c78ad03dd144637a0e398627ed1b66e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.9 MB (194900886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e093cd3a69d5df47c8a1cee16e99272e1d18ec336ed2fa3946b8c336e29c7ff`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 07:22:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 07:22:28 GMT
COPY dir:66cfc1773e07dead4d108eefca05e38bbe528aec6797deefc0559c5a4d41e721 in /opt/java/openjdk 
# Wed, 20 Sep 2023 07:22:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 07:22:29 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 07:22:29 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 07:22:29 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 07:22:35 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 07:22:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 07:22:35 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 07:22:54 GMT
RUN boot
# Wed, 20 Sep 2023 07:22:55 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d904e0e0acb14ab36621cdb61a83d87d553b53cafbe8016f9cc443e19e4ff9`  
		Last Modified: Wed, 20 Sep 2023 07:34:08 GMT  
		Size: 103.6 MB (103585017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cf35b44da32661093b4ddd9add983354404c7a45f367c4ec3c3d26758427f7`  
		Last Modified: Wed, 20 Sep 2023 07:33:59 GMT  
		Size: 1.1 MB (1077545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7598c6f5715661f815ee95340cc6a5108ec1514462c74b0c2b5b8d6ab9c2ae`  
		Last Modified: Wed, 20 Sep 2023 07:34:02 GMT  
		Size: 58.8 MB (58820613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b25800d24e3cec2ce5cd445a1c58f444bccdf9e55303d75d9f0f9e29a20be24f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.6 MB (192638612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f835f78d3722161828a3826fab73c0cbef188d5ca805822b602f15f30ac76c`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:48:13 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 09:48:13 GMT
COPY dir:b83f0a0f236c1f97de459c8ae266f437d3630abb3700f3b868301c8fe017c49a in /opt/java/openjdk 
# Wed, 20 Sep 2023 09:48:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 09:48:16 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 09:48:16 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 09:48:16 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 09:48:20 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 09:48:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 09:48:21 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 09:48:38 GMT
RUN boot
# Wed, 20 Sep 2023 09:48:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a2a7c9cc81fa3f64b00acd6c11ed487558b9944662fa13fd7c7a43dc53ba80`  
		Last Modified: Wed, 20 Sep 2023 09:58:05 GMT  
		Size: 102.7 MB (102690456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5166b91c0dca36e3edca660dc98598ec0c4fe59c688231be6af4609ee228bcb`  
		Last Modified: Wed, 20 Sep 2023 09:57:57 GMT  
		Size: 1.1 MB (1064835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a51ff1448fd8cac1c27f650f067ab45ce6e2c122321792878dd9dd0226fc30`  
		Last Modified: Wed, 20 Sep 2023 09:58:01 GMT  
		Size: 58.8 MB (58820452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
