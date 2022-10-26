## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:74baf8d0bf670669749550c94c0321c7b40a9916905f8aa1bbf027dd8080d866
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:206ab170afc3bcbedc9b09f33b1f0cbbdf548869731f455400c7932cb4084619
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.4 MB (308366852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6eb5e84ebdb0ed003fa50029eb2153595154af4efce2e807bf1215ca591a0ac`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:39:23 GMT
COPY dir:09afbf947759009c57336c17f70cd71239c5d8b0170793151aec66483cdd0976 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:39:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:39:24 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:39:25 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:39:25 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:39:31 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:39:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:39:31 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:39:51 GMT
RUN boot
# Tue, 25 Oct 2022 02:39:51 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 25 Oct 2022 02:39:51 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 25 Oct 2022 02:39:52 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac76dde2c2f13d28db088f654035acb0c8244b4c9447b8e9b0cfdb280fee3c55`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 192.1 MB (192137591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b634bbf12e96ba68daf84945435fe526a086f43553876baf48e5af3c163acaf6`  
		Last Modified: Tue, 25 Oct 2022 02:51:50 GMT  
		Size: 2.4 MB (2362126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbdd9bb7939290f1b09a202ddc545ea2725af3f38293de94c3a0e947a2502eb`  
		Last Modified: Tue, 25 Oct 2022 02:51:53 GMT  
		Size: 58.8 MB (58820405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bf53b921ad1cc4e71562568ffb4b60e902379b64cf95a468d5fd1c2f917c56`  
		Last Modified: Tue, 25 Oct 2022 02:51:49 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f5fe23a3bbc093ee187a252b5083248c71e56463932e59ce9a72956a3003cec3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305779013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21aa88fb64edfa76d6d50b9f0df63e45587d470f1f9d9d2b1b925dc195fea16`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 00:02:38 GMT
COPY dir:dc2bc1e50ab42c5231433386b6bc2a9cff04b310112464fb4909efc66be10627 in /opt/java/openjdk 
# Wed, 26 Oct 2022 00:02:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 00:02:42 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 00:02:42 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 00:02:42 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 00:02:47 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 00:02:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 00:02:47 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 00:03:04 GMT
RUN boot
# Wed, 26 Oct 2022 00:03:04 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 00:03:04 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 00:03:04 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254ce19cfb2bcd29a467e613d869b89fb6aba651e0f5fe81a52c75afbca7f870`  
		Last Modified: Wed, 26 Oct 2022 00:20:05 GMT  
		Size: 190.9 MB (190904052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ad8ff085a9e0c8ea3d00dde3ef06793b3d45debbfde3277298a8e7ef6d47f6`  
		Last Modified: Wed, 26 Oct 2022 00:19:53 GMT  
		Size: 2.4 MB (2352285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42426d7e3d3c0ee66f60e9a67c56c9c0656f081e6c0a5cf93e5f59cfe2780bdf`  
		Last Modified: Wed, 26 Oct 2022 00:19:55 GMT  
		Size: 58.8 MB (58820310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79f05b62942f19cd271a9a11f0806a609aba174b75ba6beb73cc26bb5194043`  
		Last Modified: Wed, 26 Oct 2022 00:19:53 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
