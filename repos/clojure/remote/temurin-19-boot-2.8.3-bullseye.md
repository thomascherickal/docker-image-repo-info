## `clojure:temurin-19-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:1a9f8574a22793903142976d08ba768360aabfc33234648bfe950782a12ff65d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b7a309529ea476e1593417e2f23cb8b6cb48ef2dd3d9db29cf0237a3998b2fb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317319798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36b76ab1323185ef470510e2eb001c4cc766c9f59ded3ca10b60c8c1f59c6a1f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:05:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:14:31 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:14:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:14:33 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 04 Feb 2023 14:14:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 04 Feb 2023 14:14:33 GMT
WORKDIR /tmp
# Sat, 04 Feb 2023 14:14:39 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 04 Feb 2023 14:14:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 04 Feb 2023 14:14:39 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 04 Feb 2023 14:14:57 GMT
RUN boot
# Sat, 04 Feb 2023 14:14:57 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 04 Feb 2023 14:14:57 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 04 Feb 2023 14:14:57 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315f8da6444a266b14b964d30d4c839b42701def1a15f9b4ccf306ed2efcc5a3`  
		Last Modified: Sat, 04 Feb 2023 14:25:40 GMT  
		Size: 201.1 MB (201112948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24a7d5cf316c719fe7bcac266330b15c61c451053868b0daa38ebc563844bf7`  
		Last Modified: Sat, 04 Feb 2023 14:25:26 GMT  
		Size: 2.4 MB (2360735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de8ea8b1f84b2e8331504be43272bf28a706eb9891f58f760ef4b9ab64b224`  
		Last Modified: Sat, 04 Feb 2023 14:25:29 GMT  
		Size: 58.8 MB (58820404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b6d420dc3d84abb6e99c000edcf89a75f0baaaa35436996d401321a3a1ee16`  
		Last Modified: Sat, 04 Feb 2023 14:25:25 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:59f366fee44e1ee1c632cc79b75747968bfb1f1002f6cd143e1792596abe46de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314708568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c1eb373ccf93b6a7a6d4d173e26e1de4a0ffd44a9d47c674baca1fadfcedc4`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 20:06:09 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Wed, 25 Jan 2023 20:06:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 20:06:13 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 25 Jan 2023 20:06:13 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 20:06:13 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 20:06:18 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 20:06:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 20:06:18 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 25 Jan 2023 20:06:34 GMT
RUN boot
# Wed, 25 Jan 2023 20:06:35 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 25 Jan 2023 20:06:35 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 25 Jan 2023 20:06:35 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb4495c3280f0c24cfdcbe41be056cc37ccfd0e65b21aa6f0680e4df849f415`  
		Last Modified: Wed, 25 Jan 2023 20:16:27 GMT  
		Size: 199.9 MB (199855198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297d4b64df5a288176cb42517dff4714a9201b296332ba7ca749c8bed403fac2`  
		Last Modified: Wed, 25 Jan 2023 20:16:15 GMT  
		Size: 2.4 MB (2350620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84369c770580997200e87773aed0fbb0b73202ed1dfe5c91933abaafa6440e7`  
		Last Modified: Wed, 25 Jan 2023 20:16:17 GMT  
		Size: 58.8 MB (58820491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa387dac54f5568746f29c64ccaefdd213e20a9f4e98fa8563242fed6face73`  
		Last Modified: Wed, 25 Jan 2023 20:16:14 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
