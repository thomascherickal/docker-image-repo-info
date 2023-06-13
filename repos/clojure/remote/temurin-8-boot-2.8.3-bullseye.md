## `clojure:temurin-8-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:20e25ee6de8b4f387934b35a7c1acdf1f82b75f05da9282aab411295bda1b3e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; amd64

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

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:23b07e2d2a08eaa914fb9ccf28cd8dc48f4849943d99ae1e4b8461b7ffaebe00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168618876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4264e9725120b561c0cdd1bfdc65b926a2a45ac09fae7c66e99609837c106074`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:50:40 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:50:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:50:41 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 04:50:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 04:50:41 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:50:46 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 04:50:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 04:50:46 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 04:51:08 GMT
RUN boot
# Tue, 13 Jun 2023 04:51:08 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcca61eb6313d4e5e7eaa5a1e052d334113c44736b5940de5eec6f3f49baaeed`  
		Last Modified: Tue, 13 Jun 2023 05:00:19 GMT  
		Size: 53.7 MB (53742661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f31771693c191dbf9d4b4aa365cdc1dfda92365d6d503225234d5cf1cf7ba4`  
		Last Modified: Tue, 13 Jun 2023 05:00:14 GMT  
		Size: 2.4 MB (2351317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ee230f412503b61f537a832cf45ba7962fb80995714fea5a9f9ace60d0d79`  
		Last Modified: Tue, 13 Jun 2023 05:00:17 GMT  
		Size: 58.8 MB (58820762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
