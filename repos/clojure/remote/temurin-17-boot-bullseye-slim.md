## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:86b144cdf87ec9b7ca9b3829942bfefb9316809bbb1d6cda1fecf4d972aa114b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:1b561caae4a82fa06f4999e24d6de521766e738e3699685d1d6166481c92065d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.9 MB (283895955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7db931b348dace6820cb23ff891cf2ecb94f05f6b7721049ece92a3feda861`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:50:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:50:17 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:50:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:50:17 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:50:22 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:50:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:50:23 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:50:41 GMT
RUN boot
# Tue, 13 Jun 2023 03:50:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:50:41 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:50:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a7c9e91b0ffc9643de28e2349594beed965ccb7100a6e5052c1a57bb75adb8`  
		Last Modified: Tue, 13 Jun 2023 03:58:52 GMT  
		Size: 1.1 MB (1077504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb92376dbb14e3792373d84f67c19afaf0eecee5d179b126f976e8ba3d86d8c1`  
		Last Modified: Tue, 13 Jun 2023 03:58:55 GMT  
		Size: 58.8 MB (58820254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23da3e790d60f0f7ae6a65e401c26c1a207e80119671118e00c03e1e1bb06dde`  
		Last Modified: Tue, 13 Jun 2023 03:58:52 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9d8eb9987a33fce422d16023e66ba4926e87d9bc71182081a414be2da61baaf6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281336125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f22ac2e2923863215713f84b511cfec03d493d79755f04ddaa4a4a257e2f6df7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:28:50 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:56:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:56:02 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 04:56:02 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 04:56:02 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:56:07 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 04:56:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 04:56:07 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 04:56:24 GMT
RUN boot
# Tue, 13 Jun 2023 04:56:24 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 04:56:24 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 04:56:24 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f1d77eefd6a268a661d8baa5ffc1f6d77b6b4e27e034496d0fb5928e86485`  
		Last Modified: Tue, 13 Jun 2023 04:30:57 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60c9d4f8b6a91ec641a6318fb2cc976bcbc85abd7480c934334a80793460654`  
		Last Modified: Tue, 13 Jun 2023 05:03:21 GMT  
		Size: 1.1 MB (1064846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f22c2e1f6bb18af753656ce2f771b80b536780d9f99506b3f217e576996c71`  
		Last Modified: Tue, 13 Jun 2023 05:03:24 GMT  
		Size: 58.8 MB (58820342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5537e7281ca7f8dc2ed0706d1cff26707fd6718bf8aa6520f0d03089c9406711`  
		Last Modified: Tue, 13 Jun 2023 05:03:21 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
