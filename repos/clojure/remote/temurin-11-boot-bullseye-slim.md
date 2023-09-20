## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:ad72afa63b4ba1776443fa37dada5be51d74d101af19ea4e9807629848eb478e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:3dcf8c3703e4df0c8be0924dab60ef9bc7ff1da3cd55658b1c19c8fca1434330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236141856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80a1aaa53920e964edb3a8bd0bb9e6a9840931c73a395a872896fa13b8859cc`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 07:22:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 07:25:26 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Wed, 20 Sep 2023 07:25:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 07:25:27 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 07:25:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 07:25:27 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 07:25:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 07:25:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 07:25:33 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 07:25:52 GMT
RUN boot
# Wed, 20 Sep 2023 07:25:52 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386a93addc060819e53101917ea458e4b015b760aeb9ab2f21c38b4ff88c1e7d`  
		Last Modified: Wed, 20 Sep 2023 07:35:54 GMT  
		Size: 144.8 MB (144826040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79cd3742f41dd715bd5934214e9276cd1aa2f6cf4062fdbf7003448a4c298b9`  
		Last Modified: Wed, 20 Sep 2023 07:35:43 GMT  
		Size: 1.1 MB (1077533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b9523b5f9ef6e3a15a67953d6e98893aaeebd55ad4a1d415b910327d7ccf5c`  
		Last Modified: Wed, 20 Sep 2023 07:35:47 GMT  
		Size: 58.8 MB (58820572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:78f8b50d804e14d8a214958bf9a968d3dd41db2bba9de72b50f064444b7b3828
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231518740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9956b166333e51045574218dca6f78f8ec6ac3a2c16dbac101b0803104d105`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:48:13 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 09:50:39 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Wed, 20 Sep 2023 09:50:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 09:50:42 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 09:50:42 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 09:50:42 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 09:50:47 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 09:50:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 09:50:47 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 09:51:05 GMT
RUN boot
# Wed, 20 Sep 2023 09:51:05 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5592f56c0b958f5207a05c39e6864c0e5ea5d70e2108545808c95ea7c77904e`  
		Last Modified: Wed, 20 Sep 2023 09:59:38 GMT  
		Size: 141.6 MB (141570390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ee8cf7d98d25eaa3b65eafe31d1c9171c17128b2890943526953724e61bc08`  
		Last Modified: Wed, 20 Sep 2023 09:59:30 GMT  
		Size: 1.1 MB (1064823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207a4bb7d0c9f4c78446a41791379b4ec2d0f265808aa6c44d4e726a9de5a6ca`  
		Last Modified: Wed, 20 Sep 2023 09:59:34 GMT  
		Size: 58.8 MB (58820658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
