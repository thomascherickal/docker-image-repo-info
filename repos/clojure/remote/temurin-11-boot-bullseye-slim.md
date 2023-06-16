## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:4fa8eb743d484e41c54627a8db86a0bf3966ed35b85c37c51bc493911428e344
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:814ba745a58acec2b2e32fcbea488063ce78e8b0ea904f0809874e9e70e8f8ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289865158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbea70a22200df1bb61d7d4c890265f8b88dc276932b2420e797ec7f79474736`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:47:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:47:31 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:47:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:47:31 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:47:36 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:47:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:47:36 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:47:54 GMT
RUN boot
# Tue, 13 Jun 2023 03:47:54 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896461db9dc8d8ddae7e64687a1ce367f7d901f4479b693b57f1d1db44f9bf49`  
		Last Modified: Tue, 13 Jun 2023 03:57:10 GMT  
		Size: 1.1 MB (1077537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e34c439c42ec7516b8fc62c481bf9cf867848409c4d1df967fc44545b0f6d9c`  
		Last Modified: Tue, 13 Jun 2023 03:57:13 GMT  
		Size: 58.8 MB (58820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c3aff149d3316a892567650274609c31ddaf6720812dd93338a76af42da712b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285272405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cb696eded0ae655d0e9273f8777643ecc6563252f0e17efd55b78dd4c439889`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 04:42:21 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Fri, 16 Jun 2023 04:42:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:42:25 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 16 Jun 2023 04:42:25 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 16 Jun 2023 04:42:25 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:42:30 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 16 Jun 2023 04:42:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 16 Jun 2023 04:42:30 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 16 Jun 2023 04:42:48 GMT
RUN boot
# Fri, 16 Jun 2023 04:42:48 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f561dc152f6d05a1820783d780247855889a7f67c10ad93e662c845bc4e04b7`  
		Last Modified: Fri, 16 Jun 2023 04:54:22 GMT  
		Size: 195.3 MB (195324188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9957a538c0553b3c09b4c375828e78554437139b0fe6baa7bfccbd3ef8874cd4`  
		Last Modified: Fri, 16 Jun 2023 04:54:11 GMT  
		Size: 1.1 MB (1064852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d35d340fb752b33a5dc7e132e8810404d3a827ec64331102dc99c4a19a68db`  
		Last Modified: Fri, 16 Jun 2023 04:54:14 GMT  
		Size: 58.8 MB (58820531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
