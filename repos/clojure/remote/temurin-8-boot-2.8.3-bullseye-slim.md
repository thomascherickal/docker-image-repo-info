## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:de19ee7b37cc2ce822c619da1b303a62526f0a69c78e1623e3ce786968ac8a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:354714b226a24f34d22324fbe1a7f658518c11494eadddf48b499da85254aea8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194833586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa914590f5235e250b40da1964928c41218726316d7dfe15d39144f0357741d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:33:27 GMT
COPY dir:300027169ac55d8fb6f67a0995ca298d5de23ab51f3dc8e227f6e221abd3d2c3 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:33:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:33:28 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:33:28 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:33:28 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:33:34 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:33:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:33:34 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:34:06 GMT
RUN boot
# Tue, 25 Oct 2022 02:34:06 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c8fc7384965746c1eff2e3c90a689ae0048d4ae23d30592f0dd0e23c474bc5`  
		Last Modified: Tue, 25 Oct 2022 02:48:26 GMT  
		Size: 103.5 MB (103513848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e761cc838647a81af74d26418b6fac8922ce80f68fb3745f8c821b74bca77835`  
		Last Modified: Tue, 25 Oct 2022 02:48:17 GMT  
		Size: 1.1 MB (1078981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039d22bc141dc11dbfe00f92a4c4f2cc06d29c76f194ea734585656856c378a1`  
		Last Modified: Tue, 25 Oct 2022 02:48:20 GMT  
		Size: 58.8 MB (58820719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1e8c6a7707b7241ebee300e6c83921c2da95456804393b359dd8afe72f01cb85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.6 MB (192564089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6791db4f59e82837c99cbb3db6edc7c2ed970eaf17e54598b33355611ea27146`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 23:53:46 GMT
COPY dir:7668b70c49687fddef57006c57f288afd02ec3ccd6cde9cbc5231ec8fb9225f1 in /opt/java/openjdk 
# Tue, 25 Oct 2022 23:53:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 23:53:48 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 23:53:48 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 23:53:48 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 23:53:53 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 23:53:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 23:53:53 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 23:54:10 GMT
RUN boot
# Tue, 25 Oct 2022 23:54:11 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ac6f2c932c449efb6a51ce32f57a8b068a89aea64c8b9c5d828f0629cf158f`  
		Last Modified: Wed, 26 Oct 2022 00:13:49 GMT  
		Size: 102.6 MB (102613480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c051e47496a70efcc41784fc255c5798b36cc8d1c46b3cd6913289bae3dce06b`  
		Last Modified: Wed, 26 Oct 2022 00:13:42 GMT  
		Size: 1.1 MB (1066353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954e38e2224f2637caad3520346b2cd2a1914761b46ba6a47a365166f6f6e9ad`  
		Last Modified: Wed, 26 Oct 2022 00:13:44 GMT  
		Size: 58.8 MB (58820346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
