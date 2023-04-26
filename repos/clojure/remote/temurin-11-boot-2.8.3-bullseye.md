## `clojure:temurin-11-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:12b36ed17e484be3da02fdbf68209f695e79d38db247a563ed37e46dfe32eaba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:50af96d877c2029ec0232f28f59df1539583cc0272a838a5512dc2d42ce509c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.8 MB (314784410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d59d6628604a91a4c94227e054e4b5f3c6300c183b4ed86c7fe6e51f56b389b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:03:36 GMT
COPY dir:df592a42a629b9630bdf0ab57a63e6c60f66d91934439985e01efbb58723e9ee in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:03:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:03:38 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:03:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:03:38 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:03:44 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:03:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:03:44 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:04:02 GMT
RUN boot
# Wed, 26 Apr 2023 20:04:03 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcef585044f2e536739897cb58b63d90fd8259705b2ea701d530f9eb0462baf4`  
		Last Modified: Wed, 26 Apr 2023 20:20:37 GMT  
		Size: 198.5 MB (198549498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af3ed88188e63333beff482312d43769425ca6f7723003c14db03ea758b10d3`  
		Last Modified: Wed, 26 Apr 2023 20:20:24 GMT  
		Size: 2.4 MB (2361805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dc4d1bc4082c9b8171cc805c58b9d3fb4d02d437362dee12ca9af488b725e2`  
		Last Modified: Wed, 26 Apr 2023 20:20:27 GMT  
		Size: 58.8 MB (58820371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b3b7c4917df2d2b5af91499489ffc121043ede327109db8c90bae012d5de7ff3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.2 MB (310201275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3143bdf16e6b2b55cc6abb51551a7adfd108c20d1ab4eb616bb36ce38483c9e9`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Apr 2023 20:38:49 GMT
COPY dir:8d5d0106b2c3fe64c4905be44080473b7828ffb48e0e107739a7ba7a3cb627cf in /opt/java/openjdk 
# Wed, 26 Apr 2023 20:38:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:38:54 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Apr 2023 20:38:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Apr 2023 20:38:54 GMT
WORKDIR /tmp
# Wed, 26 Apr 2023 20:38:59 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Apr 2023 20:38:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Apr 2023 20:38:59 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Apr 2023 20:39:15 GMT
RUN boot
# Wed, 26 Apr 2023 20:39:15 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a22163ecbf30f829b3b5126d0da1a7b5a260cf8cf99c26a802b000ed514988`  
		Last Modified: Wed, 26 Apr 2023 20:52:44 GMT  
		Size: 195.3 MB (195324206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761e15758cca3d47093b4f532fd394a30bce794972b25e11143b4becb7fcdde7`  
		Last Modified: Wed, 26 Apr 2023 20:52:33 GMT  
		Size: 2.4 MB (2351101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea90590456a3631a11a6d8d77669fdfc77f2cf228f3ec178764b4c9b12adbf42`  
		Last Modified: Wed, 26 Apr 2023 20:52:36 GMT  
		Size: 58.8 MB (58820439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
