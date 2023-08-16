## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:bf0bc53aee57fcf69de439f99f651154a5f88d73079c9702aa8b1eac6ded27c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:ee7733b7a6e8358e705d55a0ac09ab3bd7a0f5213acea27bba6f90aa27133c0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236089845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de034ac597daa5fa159ea5362afd00e2e0bf059b6f325be91b9523e48410daae`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:33:03 GMT
COPY dir:8ea3eea47bd8b9d37ce2403b2d64b2cdc0fec836a119c10ec3e4ff0bcca8bb4d in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:33:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 01:33:05 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 01:33:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 01:33:05 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 01:33:11 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 01:33:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 01:33:11 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 01:33:30 GMT
RUN boot
# Wed, 16 Aug 2023 01:33:30 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 16 Aug 2023 01:33:30 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 16 Aug 2023 01:33:31 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e3c34f08976bd478d8cdd805c9120ba7dd2aeacd5c4f019c318b1b43d14a5e`  
		Last Modified: Wed, 16 Aug 2023 01:42:50 GMT  
		Size: 144.8 MB (144773799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631e37feebb341fbd9a2158e2d69466badcfaea94da358c3a35364862fcab7b1`  
		Last Modified: Wed, 16 Aug 2023 01:42:39 GMT  
		Size: 1.1 MB (1077572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07be3b821ac2bb87229a99f8087bc45edb61413e04ed803ed5f263b2cb818457`  
		Last Modified: Wed, 16 Aug 2023 01:42:43 GMT  
		Size: 58.8 MB (58820397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0da7e3ef9d3907accc95c4f75ecfb4074f3b29a190b4afab6f72b5301ea72b`  
		Last Modified: Wed, 16 Aug 2023 01:42:38 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c64f83ed5a7350a9545d842806f957ba30711f1100ac7aa34a1aeab221ad98f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.5 MB (233486586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8eaf32b6421b04acd71a9e8c8ec0de42019c468e80e449b180c657e424bff4d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:25:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 17:25:56 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 16 Aug 2023 17:25:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 16 Aug 2023 17:25:56 GMT
WORKDIR /tmp
# Wed, 16 Aug 2023 17:26:01 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 16 Aug 2023 17:26:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 16 Aug 2023 17:26:01 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 16 Aug 2023 17:26:18 GMT
RUN boot
# Wed, 16 Aug 2023 17:26:18 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 16 Aug 2023 17:26:18 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 16 Aug 2023 17:26:18 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c50391e0a88de302d4e2796b43e4d00142e1556b8a123ceb309dee403c55c5`  
		Last Modified: Wed, 16 Aug 2023 17:34:10 GMT  
		Size: 1.1 MB (1064853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be214e36ee0d7b0d5a571c2a529248699c32f431222e4ce1592b22e703f013d`  
		Last Modified: Wed, 16 Aug 2023 17:34:15 GMT  
		Size: 58.8 MB (58820412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf68b3a0a6465a15fd5efc2d102d7b6b4c8818db164ec2d1c77d3079a8e81709`  
		Last Modified: Wed, 16 Aug 2023 17:34:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
