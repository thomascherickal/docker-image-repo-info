## `clojure:temurin-11-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:4da1e71816b39a724d5e601bc57e5ec9e00117e1707735c87bc16bf20f98a8b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:4e56041cb7848f901ee8a212c3d8c5ac74ebb8bbd90229bd018d6c1b9369efc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261067780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed8625a1ce294031278e7da08e4229b2d4b484f20c81c71602562da3720551ec`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 03:17:02 GMT
COPY dir:2fc258758bb2c25982e4c8348cffe5a1ab54f4c54e52ff852a817cdf5bd62215 in /opt/java/openjdk 
# Fri, 28 Jul 2023 03:17:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 03:17:03 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 28 Jul 2023 03:17:03 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 28 Jul 2023 03:17:03 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 03:17:08 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 28 Jul 2023 03:17:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 28 Jul 2023 03:17:09 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 28 Jul 2023 03:17:27 GMT
RUN boot
# Fri, 28 Jul 2023 03:17:27 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df166fc4715d337f554c5b6904774af766db5e850d3500e12eeafae147f25b5`  
		Last Modified: Fri, 28 Jul 2023 03:29:39 GMT  
		Size: 144.8 MB (144829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2782dd0817ff7e751ac7cd7df09cc33a27a370534e24fee77783e54db7141dc6`  
		Last Modified: Fri, 28 Jul 2023 03:29:28 GMT  
		Size: 2.4 MB (2362154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e460839bb1b401df6827b07db7e0ed6f07eabe288406ea41a9d077b1bb1b73ee`  
		Last Modified: Fri, 28 Jul 2023 03:29:31 GMT  
		Size: 58.8 MB (58820563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9dceb574994b6b07f76029421aab3134afafcabc83ba62454a96d9966aa6eadc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.4 MB (256442161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ecc495b90465ae98591c5000ded91c7b23cbb90aeda384f6c1d749b03e66d9d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:29:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:20:57 GMT
COPY dir:ddfd64e7bd36f630cd100cf454a9685f9fd0f9483467dbf7a4c9a71ab0af7089 in /opt/java/openjdk 
# Tue, 08 Aug 2023 20:21:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:21:00 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Aug 2023 20:21:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 20:21:00 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 20:21:06 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Aug 2023 20:21:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 20:21:06 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Aug 2023 20:21:23 GMT
RUN boot
# Tue, 08 Aug 2023 20:21:23 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407c6d757b759af4edf90fb98cce4e2d9dcbe1dbefa7c50cb1db816f3fc06be8`  
		Last Modified: Tue, 08 Aug 2023 20:32:30 GMT  
		Size: 141.6 MB (141565363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b45d9db29da940cbe29de049721386f23b9d028eb964a7cf6b52844fe6f212b`  
		Last Modified: Tue, 08 Aug 2023 20:32:21 GMT  
		Size: 2.4 MB (2351462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847a0ce763400512fc21f589bab52492a0d9687d3a4c670010cb8266318be9d5`  
		Last Modified: Tue, 08 Aug 2023 20:32:27 GMT  
		Size: 58.8 MB (58820546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
