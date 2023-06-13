## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:212ddd0c654882dd90d994e57fcb3fe6805a9c536ddfd6823d4177ba30789029
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:401872cf1bd005c2ea41836b838efcefe8a5baed45cf8c7f809b9037f8aa5f38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170880237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d32f738a2ce2cd6d17f2d8cb31295192ed8651554f77435fc7214d60ea369ab3`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:43:40 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:43:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:43:41 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:43:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:43:41 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:43:47 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:43:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:43:47 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:44:26 GMT
RUN boot
# Tue, 13 Jun 2023 03:44:27 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea2a5521481b9bca3bce0dfdda28d5d603b3d647027901d7c767f2eda4532d3`  
		Last Modified: Tue, 13 Jun 2023 03:55:22 GMT  
		Size: 54.6 MB (54642105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c218a5f61c895882345f876ef11398ca95a4cec56e1ddba832fc39057bb940`  
		Last Modified: Tue, 13 Jun 2023 03:55:16 GMT  
		Size: 2.4 MB (2362047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af808a1d09c38b1d6d5a081838c95dd7a74f0516027dcdf64310a74d89f56f9`  
		Last Modified: Tue, 13 Jun 2023 03:55:19 GMT  
		Size: 58.8 MB (58820923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ae03b53cf9eb41a6e1bcf9f661a8cb642ca625f52ddd0c803a9090c8cb34dc72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168607130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9474315b574e4667b3cccbe6a88fcb7355a7c2d5b6ad231e2d9f427829c2b7`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:24:11 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Tue, 23 May 2023 01:24:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:24:12 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 23 May 2023 01:24:12 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:24:12 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:24:17 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 23 May 2023 01:24:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:24:18 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 23 May 2023 01:24:50 GMT
RUN boot
# Tue, 23 May 2023 01:24:51 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec933d3080ef0a9a725f147ed686986ad36ef60808bf5f0ed2091007522988c`  
		Last Modified: Tue, 23 May 2023 01:34:03 GMT  
		Size: 53.7 MB (53742673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070959a9f233868fc78ef05bae1acb49aba6d3df875b0f4e7cf339f7e6715fd`  
		Last Modified: Tue, 23 May 2023 01:33:59 GMT  
		Size: 2.4 MB (2351112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0529d8976c41b9274b951b8bcfeee0fd4e000a4228ff878962f98c816f7ec201`  
		Last Modified: Tue, 23 May 2023 01:34:01 GMT  
		Size: 58.8 MB (58820733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
