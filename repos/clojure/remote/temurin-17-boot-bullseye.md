## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:a0f97d738692fd41d3d48fdde4cc6ed176055e62a2aed2cd683356b6b1e20584
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:0bf2251a954d7f9e814afebc36d5ac14f0b78b629a3bfd353200c4ea050a34e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.8 MB (308818483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be49191777260afbb1389acdc165036ad80b255e33cacba473e340dc7012fa7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:49:42 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:49:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:49:44 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:49:44 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:49:44 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:49:49 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:49:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:49:49 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:50:08 GMT
RUN boot
# Tue, 13 Jun 2023 03:50:08 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:50:08 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:50:08 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d42f641d3e7c6f97669559265ce43b9d70845285e59b903d626111efdf96ff`  
		Last Modified: Tue, 13 Jun 2023 03:58:44 GMT  
		Size: 192.6 MB (192580397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb11fcf300dd56a0d76272aa6ad0e7dcd32acd43e5755ef13a316c8a319e7eca`  
		Last Modified: Tue, 13 Jun 2023 03:58:30 GMT  
		Size: 2.4 MB (2361979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29755cf6bc928717fd2466cf52c997ad041eb2a9c3925844f8c75560236edbf7`  
		Last Modified: Tue, 13 Jun 2023 03:58:33 GMT  
		Size: 58.8 MB (58820548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb066ebb7b6e53d73a2618ecdb7fb6b4b96b310a326e7d03bcfd2f4eba4978c1`  
		Last Modified: Tue, 13 Jun 2023 03:58:30 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6411c8fa1af47017998a971e46d5d74cc4af554e980329da73d84adbbea29cc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306263931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d42ee4c7dc2fe1b83e1ea78ac48188103d64aa809c7a5afe3cd8edb0eeb3431`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 04:46:29 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Fri, 16 Jun 2023 04:46:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:46:33 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 16 Jun 2023 04:46:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 16 Jun 2023 04:46:33 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:46:38 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 16 Jun 2023 04:46:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 16 Jun 2023 04:46:38 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 16 Jun 2023 04:46:56 GMT
RUN boot
# Fri, 16 Jun 2023 04:46:56 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 16 Jun 2023 04:46:56 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 16 Jun 2023 04:46:56 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172252176b2d2b44f66626001ffedf36355c238558bbc403980303e6b6c92ae9`  
		Last Modified: Fri, 16 Jun 2023 04:56:58 GMT  
		Size: 191.4 MB (191387640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d209f9a9a585297e98927ab8aece778729273ea765bf993bb6486bf27fb93c`  
		Last Modified: Fri, 16 Jun 2023 04:56:47 GMT  
		Size: 2.4 MB (2351326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7b155d8f7d2e9e0af3797d52f2d75d2183be3414ac33775d731a870d7199d0`  
		Last Modified: Fri, 16 Jun 2023 04:56:50 GMT  
		Size: 58.8 MB (58820431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29a311b04bd6c06a341b1cb4a27fae423071a6c36312dead7470b3f4208df1d`  
		Last Modified: Fri, 16 Jun 2023 04:56:46 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
