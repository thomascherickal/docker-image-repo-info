## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:48a026516b05d57e8b99a126a9db18a68feab321c358c915f22d4041bbbbc8cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:5872499d4479874a2ed7aaabaa1e1e36d6d5fa1e32fa39deee10174621a1694e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236092013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e82ea8433faaa6c86e7646178f3b8a08b0267f8b2c8ed4c8ffbf1c47d5cad96b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 20:48:51 GMT
COPY dir:6777d1f77166c2ecdd8f4eb23f5fd82574aa8a90fd65d6dff981fbb31778a3d1 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:31:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:31:49 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 31 Aug 2023 23:31:49 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 31 Aug 2023 23:31:49 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:31:54 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 31 Aug 2023 23:31:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 31 Aug 2023 23:31:54 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 31 Aug 2023 23:32:13 GMT
RUN boot
# Thu, 31 Aug 2023 23:32:14 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 31 Aug 2023 23:32:14 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 31 Aug 2023 23:32:14 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65006a4851e206ccc53a9bf891b081e6fefbdbe0fcb897d670970fc7f2eff9ea`  
		Last Modified: Thu, 31 Aug 2023 20:51:41 GMT  
		Size: 144.8 MB (144775820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da35ef5d3ba3f1252a68755d0ce1a97b682682fedaa79a100eb40ba9f34bb3a9`  
		Last Modified: Thu, 31 Aug 2023 23:44:30 GMT  
		Size: 1.1 MB (1077543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad62d6d787003da538724e450fa06ddf7484b999164234d6983ef71a44a6598b`  
		Last Modified: Thu, 31 Aug 2023 23:44:33 GMT  
		Size: 58.8 MB (58820573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa86b440bd8ee4a418cd069ee84f98f4022f58f2e36c433f7e6e808aaf64bda`  
		Last Modified: Thu, 31 Aug 2023 23:44:29 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:14e0d778dbcf89f0cbded29a619e74e9e948accaa74993665ddefb07636b9655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.5 MB (233492105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ac48bbbc0017a9ebee9cd2108eed9bd0d5e514bf3411db264d8f0a1ff1b07f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:48:00 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:48:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:48:04 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Sep 2023 01:48:04 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Sep 2023 01:48:04 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:48:08 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Sep 2023 01:48:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Sep 2023 01:48:09 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Sep 2023 01:48:25 GMT
RUN boot
# Sat, 02 Sep 2023 01:48:26 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 02 Sep 2023 01:48:26 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 02 Sep 2023 01:48:26 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75390d7bc4a96162e240272aeff28881955f7af498179aa85faecd879748f913`  
		Last Modified: Sat, 02 Sep 2023 01:55:46 GMT  
		Size: 143.5 MB (143543515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6609d00c40d78b8dfbbef7aecbccb296e31409a782e41d7c2eb33229765bdf6`  
		Last Modified: Sat, 02 Sep 2023 01:55:37 GMT  
		Size: 1.1 MB (1064830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c463f0425e6740b6d9abdb541b3a8129352472b86b9506031c099ef10da4c69`  
		Last Modified: Sat, 02 Sep 2023 01:55:39 GMT  
		Size: 58.8 MB (58820544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fe3c7d5e4d5ae1b7c61d7bd7c47f88113b7f6ae2d6f9540d47f8b1a29b5e17`  
		Last Modified: Sat, 02 Sep 2023 01:55:36 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
