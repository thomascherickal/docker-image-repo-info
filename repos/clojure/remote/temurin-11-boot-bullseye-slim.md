## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:9a7e0f0f116503059041d22d862e973ac770381a206dbcf58242b25b599d5b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:1593be410986b0f0d074ce554d7d57d8459a52d5522a98a3bb559bf2c282ce6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289785340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f107b5648e85407c9d516ad418b35e451f5cfaa7bb370e056b2f62fc7ec2741b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:20:31 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:20:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:20:32 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:20:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:20:33 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:20:38 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:20:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:20:38 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:20:55 GMT
RUN boot
# Thu, 23 Mar 2023 06:20:56 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1504cbd1d7ea21f45a7c90d9e13b13742e330dcd47fdbe975ca32319c2681080`  
		Last Modified: Thu, 23 Mar 2023 06:31:09 GMT  
		Size: 198.5 MB (198476003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92414d4a91eceed1599f828ad2d28440113e07cdcaa895664eda6f720a0b683a`  
		Last Modified: Thu, 23 Mar 2023 06:30:55 GMT  
		Size: 1.1 MB (1077345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eb20615d9ec8dd731e6f9e474e9cba572cbbdb7962629581dffb984ac2e4b8`  
		Last Modified: Thu, 23 Mar 2023 06:30:59 GMT  
		Size: 58.8 MB (58820587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:7a8ff05ce985c5beffadf449a78426a1bf69f7f9eb6848074ff7dd55c5e22ace
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285190360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69266b231345b1e293b440630570ce5f61a3f4e8b434b3d237e6411b58d58e6a`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:55:00 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:55:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:55:05 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:55:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:55:05 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:55:09 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:55:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:55:09 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:55:26 GMT
RUN boot
# Thu, 23 Mar 2023 06:55:26 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10110f881fd4b5d631a0d4a395c31433fb4f28f016302e6eac7248a1e22335b`  
		Last Modified: Thu, 23 Mar 2023 07:04:27 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28396d5e0f3bdeac953a158c45dbac8ca2624055aa61b477f565d1860bccd63`  
		Last Modified: Thu, 23 Mar 2023 07:04:17 GMT  
		Size: 1.1 MB (1064637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5cdc42a109c59af91f49d130b0b48968c39a9ceded1a50f55f52d832f45985`  
		Last Modified: Thu, 23 Mar 2023 07:04:19 GMT  
		Size: 58.8 MB (58820516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
