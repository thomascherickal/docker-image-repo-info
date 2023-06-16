## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:e0bfed07c0eeb57c9e8247fa72414afab43e7c8300e8addea86a91150be5a211
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:026ef70cd1ab7bea3bd8e2788e2e57df1a94df0802e7fcdcc6577d2bf40e95b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314787433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17bbbb8b973dfea5aecea85404d16c6e46fa93d92e3a3555f789490bb3113b45`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:46:56 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:46:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:46:57 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:46:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:46:58 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:47:03 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:47:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:47:03 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:47:23 GMT
RUN boot
# Tue, 13 Jun 2023 03:47:23 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12b8c3d504afe22ba8eb61403c46f5cc24b3d13561e5bdd23c0feed04b5a618`  
		Last Modified: Tue, 13 Jun 2023 03:57:02 GMT  
		Size: 198.5 MB (198549757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469c62e203ad725f6718a3cfbb7d7aa9551693af7dc52b415fb327da67663754`  
		Last Modified: Tue, 13 Jun 2023 03:56:48 GMT  
		Size: 2.4 MB (2362063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8212518e31e30a33dc2aff96b24baf7797e97bca491e7ca9e8a88acba229fe3`  
		Last Modified: Tue, 13 Jun 2023 03:56:51 GMT  
		Size: 58.8 MB (58820451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d04067274042e13cc6c1486418d4dbf6492195e58289eab714146db12bf08744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.2 MB (310200225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a92afdfe414f409f8b5172cbf2ed330ccd2f75829c027f25356b35b4eb0eede`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 04:41:42 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Fri, 16 Jun 2023 04:41:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:41:46 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 16 Jun 2023 04:41:47 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 16 Jun 2023 04:41:47 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:41:56 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 16 Jun 2023 04:41:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 16 Jun 2023 04:41:56 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 16 Jun 2023 04:42:14 GMT
RUN boot
# Fri, 16 Jun 2023 04:42:14 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b429dc913a313200e2709dc18ae8c848cf538439e00d089ddee5b4541385cd44`  
		Last Modified: Fri, 16 Jun 2023 04:54:03 GMT  
		Size: 195.3 MB (195324188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf71a08da7f244340b9830b1ca93d79f63ac4fa070dc7c70c3abeefa93dcf31`  
		Last Modified: Fri, 16 Jun 2023 04:53:52 GMT  
		Size: 2.4 MB (2351346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84315f8cf675e5ebc8e532fa123e6a35f24c1eb9a5c3d9a0b512bb8294e4ade9`  
		Last Modified: Fri, 16 Jun 2023 04:53:55 GMT  
		Size: 58.8 MB (58820555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
