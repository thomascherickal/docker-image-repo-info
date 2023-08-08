## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:99bd2821940c5f3c9ac3ae887949ddf55da1cdb5b95ec48b68b2c333801d4bdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:52411a7c5e77eac24b4f85e97785c0f9a261c95165d26ce2138a4914f579ac91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236145306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6b6fc560de194cf1237e2fdac4c32a7e8aa25cd9ea461c33cf5e2bb8b0f3bb`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:22:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 02:22:57 GMT
COPY dir:2fc258758bb2c25982e4c8348cffe5a1ab54f4c54e52ff852a817cdf5bd62215 in /opt/java/openjdk 
# Fri, 28 Jul 2023 03:17:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 03:17:34 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 28 Jul 2023 03:17:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 28 Jul 2023 03:17:35 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 03:17:40 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 28 Jul 2023 03:17:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 28 Jul 2023 03:17:40 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 28 Jul 2023 03:17:59 GMT
RUN boot
# Fri, 28 Jul 2023 03:17:59 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8093463543ce0d2e4cc72a5011db04a63e89f8a49c37702622adc8e1defc155b`  
		Last Modified: Fri, 28 Jul 2023 02:25:48 GMT  
		Size: 144.8 MB (144829555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a36de60b1b40a40ec943d157c4474d2fb8a6d5c5b74ed1d6a7f7cebff6c00b9`  
		Last Modified: Fri, 28 Jul 2023 03:29:48 GMT  
		Size: 1.1 MB (1077551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ade44ace5ef322b2c1d7c99869d1c7eb473670d332120fb8f4de2729868566`  
		Last Modified: Fri, 28 Jul 2023 03:29:53 GMT  
		Size: 58.8 MB (58820598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:373e80d7e573c9eed26d6047587d5844cecb1b3d66949b51e2151428bacd7a33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231513512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ab4f3b4d1b9c42ff834822e277f5d2a74ab8bb6155a8a5a1f9ac44f494cb55`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:25:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:21:30 GMT
COPY dir:ddfd64e7bd36f630cd100cf454a9685f9fd0f9483467dbf7a4c9a71ab0af7089 in /opt/java/openjdk 
# Tue, 08 Aug 2023 20:21:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:21:34 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Aug 2023 20:21:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 20:21:34 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 20:21:38 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Aug 2023 20:21:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 20:21:38 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Aug 2023 20:21:56 GMT
RUN boot
# Tue, 08 Aug 2023 20:21:56 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4618d52dbf5263b6400122ab8ead6b84fd0a5fdd684ed03f8e4a606dff09c08e`  
		Last Modified: Tue, 08 Aug 2023 20:32:48 GMT  
		Size: 141.6 MB (141565379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192d454ecfed08a1b61e9911139b0ffef4a3897a68181684bd86623aaf6e681f`  
		Last Modified: Tue, 08 Aug 2023 20:32:41 GMT  
		Size: 1.1 MB (1064804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c1dfb06cf77b37ff206d59dbdc2b13986eaaebb33c03e7563717466cbf7a5`  
		Last Modified: Tue, 08 Aug 2023 20:32:45 GMT  
		Size: 58.8 MB (58820498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
