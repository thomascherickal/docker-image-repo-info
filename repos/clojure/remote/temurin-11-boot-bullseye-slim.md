## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:0eb30099985df2e76f82f2bc62236b2426464ba83bcda1bab577e88c58f42ffd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:615727caf63203931bd97e678484cad3cb525d4612a40aafb5dc1aecf3137f52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236147228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7149e637d1335b44b48f62b67d84134808c56bd2f143f0a5cc91588b662f7d75`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:29:58 GMT
COPY dir:071e7267c24117f41caea93a03f9d7c7d8dc1c681571e9b8f2b8b433c86f9778 in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:30:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 01:30:00 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 01:30:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 01:30:00 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 01:30:06 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 01:30:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 01:30:06 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 01:30:25 GMT
RUN boot
# Wed, 16 Aug 2023 01:30:25 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3d4d2f5867a303bd00d8ec72e811cf9b8a3162b30a9f4488f6f70d93a67480`  
		Last Modified: Wed, 16 Aug 2023 01:41:00 GMT  
		Size: 144.8 MB (144831559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd12f59561877110c19cff04c64c1d8fb872aed5f049abc13b4f46873bab19`  
		Last Modified: Wed, 16 Aug 2023 01:40:48 GMT  
		Size: 1.1 MB (1077559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bfef1eb8f0de8fbb2f7482d40f4f8e85efbdae766c1c74efa92826b61541fd`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 58.8 MB (58820432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b5c96fafc85f63b0895ef443eaeac51f4cdf6c3b922c62213f5d993c66c43c35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231513357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c775fcbf320f7acd8ea7cd59f00f00935d1c475d246e782941f0e90336f443`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:49:18 GMT
COPY dir:ddfd64e7bd36f630cd100cf454a9685f9fd0f9483467dbf7a4c9a71ab0af7089 in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:49:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 01:49:21 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 01:49:21 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 01:49:21 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 01:49:26 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 01:49:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 01:49:26 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 01:49:42 GMT
RUN boot
# Wed, 16 Aug 2023 01:49:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5915e7301fef59f2e12ff809f83b0ddfca231cc7c25cbc8e76e79541f65928a8`  
		Last Modified: Wed, 16 Aug 2023 01:58:02 GMT  
		Size: 141.6 MB (141565378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0075d282ba033d4325d59d37b6c4e78aba220c50f738748c55fae3ae376776`  
		Last Modified: Wed, 16 Aug 2023 01:57:53 GMT  
		Size: 1.1 MB (1064832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b166626f6eeb99c6f3541761636715cc8f28e7c252f69fbb2c6bd535908563`  
		Last Modified: Wed, 16 Aug 2023 01:57:56 GMT  
		Size: 58.8 MB (58820331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
