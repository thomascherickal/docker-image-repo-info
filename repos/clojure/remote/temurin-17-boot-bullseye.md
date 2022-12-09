## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:1d377ef4c3d38a4347018d30bb87c28c762a11a3aa838af3383fb2f25cf9649e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:e4717ca5c485f048629edf464866eea07f032151d115ba8305851acc4493aaa5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308655353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f39dd8b4fe0b8596a65b1a30b315f10dbd630233c687fbdf7397e43a93b9865`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:41:36 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:41:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:41:38 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 06:41:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 06:41:38 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:41:44 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 06:41:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 06:41:44 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 06:42:02 GMT
RUN boot
# Fri, 09 Dec 2022 06:42:02 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 06:42:02 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 06:42:02 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd66dd8de79208b3ac1ba78188137da46ecd5c4585e3964d2bf9fe06372b58aa`  
		Last Modified: Fri, 09 Dec 2022 06:56:44 GMT  
		Size: 192.4 MB (192431275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea397b01663fdd9aedffd20ce4262789fd3de5d2fc814b075b28d9d66039926`  
		Last Modified: Fri, 09 Dec 2022 06:56:30 GMT  
		Size: 2.4 MB (2362017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56764baa4b35a16f8ac8548bd8dca667a739a2877912e32f4bcfb6ebe230bf43`  
		Last Modified: Fri, 09 Dec 2022 06:56:33 GMT  
		Size: 58.8 MB (58820319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511c492b73e31b87d2277e4b70d777b746fe0ee77294c905978b6c70a98ceddd`  
		Last Modified: Fri, 09 Dec 2022 06:56:29 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8e6996b7729db9d4cd0023f5a6ea915c0bfaa187ea6173a78acc92826aa7a37c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306087562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35d6da315471c1699ed7fb176f790bb82035b4b6cbd39154770dc429bca818f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:07:54 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:07:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 05:07:58 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 05:07:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 05:07:58 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:08:03 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 05:08:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 05:08:03 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 05:08:19 GMT
RUN boot
# Fri, 09 Dec 2022 05:08:20 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 05:08:20 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 05:08:20 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e87ae6358ff8aab3fb41f68232225878ffb398969ae416f8e58ce122fdb05`  
		Last Modified: Fri, 09 Dec 2022 05:21:15 GMT  
		Size: 191.2 MB (191215204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996964e23ccb9ca71fc208b28e992900457c8db65158ef607a997ba5fcca4d8e`  
		Last Modified: Fri, 09 Dec 2022 05:21:04 GMT  
		Size: 2.4 MB (2352318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6033497af48540a65b213cccd589b0fa1609173afc47153ab4a0af5a1003e40d`  
		Last Modified: Fri, 09 Dec 2022 05:21:06 GMT  
		Size: 58.8 MB (58820494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81864a057480de24c15df01360e859409ff0abfa036fbcd06d075ecc104e01a0`  
		Last Modified: Fri, 09 Dec 2022 05:21:03 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
