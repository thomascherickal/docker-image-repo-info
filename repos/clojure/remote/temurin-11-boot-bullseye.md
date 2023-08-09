## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:330797d95289ea6d31852682b736a49a3f053bb74aef1395da28a5eed9a5a6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:456da77a86921d472e3c031c849b93347a77418d2b8f527702bfdb6c4fc50ba3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261069730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e72cec0415caaf82ddf55d6d66c69e32b1cb7f503bf126ab17bfede63b56ed`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 22:29:36 GMT
COPY dir:071e7267c24117f41caea93a03f9d7c7d8dc1c681571e9b8f2b8b433c86f9778 in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:29:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:29:37 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Aug 2023 22:29:37 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 22:29:37 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 22:29:43 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Aug 2023 22:29:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 22:29:43 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Aug 2023 22:30:03 GMT
RUN boot
# Tue, 08 Aug 2023 22:30:03 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a4eb0585d7c0fad1a2cb76388ee1ecc94aa2230b3e8084d56c17968d0ef2f`  
		Last Modified: Tue, 08 Aug 2023 22:46:07 GMT  
		Size: 144.8 MB (144831528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48299391ee4034a27c3ca75daa2b5ee5e06c03888b1fdb181d9bc7359d580c50`  
		Last Modified: Tue, 08 Aug 2023 22:45:53 GMT  
		Size: 2.4 MB (2362182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d80c172de5458adc7e42a5d6e7ed53459c83d1045dc803d4bebd992e85228d`  
		Last Modified: Tue, 08 Aug 2023 22:45:58 GMT  
		Size: 58.8 MB (58820449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

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
