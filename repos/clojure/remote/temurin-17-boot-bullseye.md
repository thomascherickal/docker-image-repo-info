## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:9232aa36c86f791a0e89758966e530637dd358827816ffa3bf8c219a33d30569
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:9e49d3648b6006d9d3079429b8cff413f12ebd45f8a900807926c72e1c084f80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308666390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b800d0c505b18061a282399b5ce6021c0740e264f9544a5bcdf4e6cc60d5544`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:16:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:22:38 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:22:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:22:40 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:22:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:22:40 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:22:46 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:22:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:22:46 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:23:03 GMT
RUN boot
# Thu, 23 Mar 2023 06:23:03 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:23:03 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:23:04 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b6efe2710f8afbae0603df0d04f44f97f99a0a0a87709cad6c690fb01572d`  
		Last Modified: Thu, 23 Mar 2023 06:32:29 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cf0ff3bdfe63d9c3313e7d2fc8488205c6d76ba227d9d0264b4e75faa7d6c3`  
		Last Modified: Thu, 23 Mar 2023 06:32:16 GMT  
		Size: 2.4 MB (2361571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973bc8e6b4e4175ca9c33f6038aedccf10f3733f298bd8df5ce444eb48ac8668`  
		Last Modified: Thu, 23 Mar 2023 06:32:19 GMT  
		Size: 58.8 MB (58820548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d85b76a7acf0f226438b4e46ae8d43e1023213861a7a971198a16d593130e6`  
		Last Modified: Thu, 23 Mar 2023 06:32:15 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8e96ed79be8f7c8ed347e138c163a04d8368527ce690182e8aa988ade247f93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306135478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3539a296aaa7227e3e03c39ee1dfd66fda988c307b3215f89c4832d77aa6df2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:56:51 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:56:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:56:56 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:56:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:56:56 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:57:00 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:57:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:57:01 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:57:16 GMT
RUN boot
# Thu, 23 Mar 2023 06:57:16 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:57:17 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:57:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20e4c5710ab51796871e20e42a7c05e81d5c06c45eaa73fb32bce80bac1c808`  
		Last Modified: Thu, 23 Mar 2023 07:05:41 GMT  
		Size: 191.3 MB (191260430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628af8dabb7a30032c2d9e1ea1342f98813e6d90563ca92f20c3b918e54fed8d`  
		Last Modified: Thu, 23 Mar 2023 07:05:31 GMT  
		Size: 2.4 MB (2350987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20e3a687214b5de098e1e5d4225925e4a3b4a237cef3c31eee8360afc158628`  
		Last Modified: Thu, 23 Mar 2023 07:05:33 GMT  
		Size: 58.8 MB (58820562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2de4bf47e13aadb54790e7a99f7b1a87ecafa40035baa0b3fa06268c860de14`  
		Last Modified: Thu, 23 Mar 2023 07:05:30 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
