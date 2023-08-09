## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:a84ac7e0b3e4cd8ff19648739e75111697eb662716b2289af1d0384975bf88b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:23ca20464e7f0cd6d6364b21ab4576db51effb9c361d0e09600397296d935174
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236147253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb414b0f52fa8effecd2d8a6225443d8cc6c998ba54d3af46342af137a69660f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:22:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:19:21 GMT
COPY dir:071e7267c24117f41caea93a03f9d7c7d8dc1c681571e9b8f2b8b433c86f9778 in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:30:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:30:09 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 08 Aug 2023 22:30:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 22:30:09 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 22:30:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 08 Aug 2023 22:30:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 22:30:14 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 08 Aug 2023 22:30:34 GMT
RUN boot
# Tue, 08 Aug 2023 22:30:34 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a67c0c0e120eaa60971623d0bcdd60c592fdaff036504dc7443ce6dac2118`  
		Last Modified: Tue, 08 Aug 2023 20:23:28 GMT  
		Size: 144.8 MB (144831527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c9140e95e625ec90c937b4f28d1fd0f20220535db5a8e957423dba74331c83`  
		Last Modified: Tue, 08 Aug 2023 22:46:16 GMT  
		Size: 1.1 MB (1077531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07729eea219ab56d43182e644d6176bb6661bce200d20903c5d108b6d8d2b885`  
		Last Modified: Tue, 08 Aug 2023 22:46:20 GMT  
		Size: 58.8 MB (58820593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

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
