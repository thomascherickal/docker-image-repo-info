## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:ce0221d05b632ce839412afdcd2ccd8bcb5109a04d57449786136782815b857e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

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

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:78d8847f29ff1a300a19bb717c0c57acd7f39898d8b47c3332e4285baca5644c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306264102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc898ede61c4bca137b8a1d0234d2d0b84bc64122fab3c7ba144d6c52cf1a13`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:55:30 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:55:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:55:34 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 04:55:34 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 04:55:34 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:55:39 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 04:55:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 04:55:39 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 04:55:55 GMT
RUN boot
# Tue, 13 Jun 2023 04:55:55 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 04:55:56 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 04:55:56 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2f5c11cf1de6e6cdfa958273d80e09d9e847bc2a31fc5ff8ab8ff58dfecc86`  
		Last Modified: Tue, 13 Jun 2023 05:03:13 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3876f68d4e22c6414f1133404ee1f8a09b3063241ee609d77cee222d5b501ca6`  
		Last Modified: Tue, 13 Jun 2023 05:03:02 GMT  
		Size: 2.4 MB (2351322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033d7c0ae0c65c888314daa178a81ba925bc47d262a49551f564e03d04ddc906`  
		Last Modified: Tue, 13 Jun 2023 05:03:04 GMT  
		Size: 58.8 MB (58820541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08c13162b4ea73bc52d41e28ed02f04d11ff00735b7abe5c6bf04717af6c2a2`  
		Last Modified: Tue, 13 Jun 2023 05:03:01 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
