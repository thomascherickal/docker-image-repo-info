## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:b0b780884febef86234c63e7f239d7eff3cf6df860361a3ed1ba80bb253fd260
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:84c4a962fec9b208792d6e207d49315991b48c101a5c87001136a55c5a17797d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.8 MB (308815726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcb5f35cace5787bbc2ba2b606fdc5a63e348294972d424abf83ad3098183af`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:08:38 GMT
COPY dir:097a611561277927a8e367a60640ce12877b7a6373689dec24d5cfb76f99c807 in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:08:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:08:40 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:08:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:08:40 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:08:46 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:08:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:08:46 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:09:03 GMT
RUN boot
# Wed, 26 Apr 2023 20:09:03 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Apr 2023 20:09:04 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Apr 2023 20:09:04 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e363e191094639c858d95dc4482d74ded984d3d69a9dc0e9278ea1712a1c3b51`  
		Last Modified: Wed, 26 Apr 2023 20:24:02 GMT  
		Size: 192.6 MB (192580410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53de5e74f321f4bd28bece1c35b577d1d18fbff53e50cbc17e0fb33189d0b5d7`  
		Last Modified: Wed, 26 Apr 2023 20:23:49 GMT  
		Size: 2.4 MB (2361739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d633b3657664ef54bc6ebb18d265417ccfc025ae317cb20266af26ee709c95`  
		Last Modified: Wed, 26 Apr 2023 20:23:52 GMT  
		Size: 58.8 MB (58820442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c8a532960a09074c6f7d7bdcf762acedca73d4147092674251074c0df2f265`  
		Last Modified: Wed, 26 Apr 2023 20:23:48 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e362f41a0fa5c571e32c809aea977a072f31f345ec1a21552f7398bd717e125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306264968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31448eb213187bb05e603d33b2b45211d53b6f1842b0bb5e2c3a3a1ddee8bbc2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:42:59 GMT
COPY dir:d3d9f08d06fd1214b20f5d901cee398f498773bedf69f0d3cc795772967cfe44 in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:43:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:43:02 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:43:02 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:43:02 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:43:07 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:43:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:43:08 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:43:24 GMT
RUN boot
# Wed, 26 Apr 2023 20:43:24 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 26 Apr 2023 20:43:24 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Apr 2023 20:43:24 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5d8dfe56c9a11e21f9a4447bec8b6fff80781ad18ef5c0814bc9af24fd24d1`  
		Last Modified: Wed, 26 Apr 2023 20:55:30 GMT  
		Size: 191.4 MB (191387667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8291f5987d5049d64f7595eb6c83fc44c5fa93640eeb68888223855b60050aa0`  
		Last Modified: Wed, 26 Apr 2023 20:55:19 GMT  
		Size: 2.4 MB (2351093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd416d7e4eb39ab95eac6aa2fadf6b6a054b8aef73c1b1cee203e447cf4de8b`  
		Last Modified: Wed, 26 Apr 2023 20:55:22 GMT  
		Size: 58.8 MB (58820279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18c33d9528569ca9e2f95533d245f3aec91e1047bf3c9822ec053294643e60a`  
		Last Modified: Wed, 26 Apr 2023 20:55:19 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
