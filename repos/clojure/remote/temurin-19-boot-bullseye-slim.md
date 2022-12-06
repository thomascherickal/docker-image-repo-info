## `clojure:temurin-19-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:d7b6ab3c4712c79ea1dad1e3c7a263cbcf26ad5b8c32da4c9ce70958f66535d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a49e618dba367f1ea0841117de578cd7e93d6f6f32fc31a9205b0d1d7262393e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292416041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe4fce2e2a09f8488980b4af42cadcef9794473baad0f23b31f73a959932e83`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:58:15 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:58:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:58:17 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:58:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:58:17 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:58:23 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:58:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:58:23 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:58:41 GMT
RUN boot
# Tue, 06 Dec 2022 01:58:41 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 01:58:41 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 01:58:41 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f07ccb399757ca2eb22ecfbed8b8e0fe753148c9c99205f4b73d03bcc43ef0d`  
		Last Modified: Tue, 06 Dec 2022 02:09:27 GMT  
		Size: 201.1 MB (201103429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061637c2a8ef138f02b7c0a9e251e5c03d302172c448f8bae60d3a32033a1513`  
		Last Modified: Tue, 06 Dec 2022 02:09:11 GMT  
		Size: 1.1 MB (1078970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fca135a9b513a7ba7e1894685d32ea9e4240ae69cfa636529f54db90a940ba`  
		Last Modified: Tue, 06 Dec 2022 02:09:15 GMT  
		Size: 58.8 MB (58820390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb43be7fe185f5c5855dfccc776038ef4083ae2730a87db80b613cd43e42207`  
		Last Modified: Tue, 06 Dec 2022 02:09:11 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:036cf202874438da449272d9f4130ec78ad5ddf375dd5b4c3047b0781f1e6116
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289811935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44b87cfdebd9f019b1f2f932abbb7276d8af057e09c4207d9939160381a1915b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:25:30 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:25:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:25:35 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:25:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:25:35 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:25:40 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:25:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:25:40 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:25:57 GMT
RUN boot
# Tue, 06 Dec 2022 02:25:57 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:25:57 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:25:58 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41824f9c81730654da632df65bb8c2a4392976f97f4a938f885db8e2cb6804c2`  
		Last Modified: Tue, 06 Dec 2022 02:35:24 GMT  
		Size: 199.9 MB (199864417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a002266f34b4a793cef4eecb67120a28e0d2ec6ec45b75c6952b0c76f6e3fb`  
		Last Modified: Tue, 06 Dec 2022 02:35:11 GMT  
		Size: 1.1 MB (1066350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0381e5e5f036ad5dfe1ec6ba150895ce8c02dfd2401120f3dd165ea82fc2b2d`  
		Last Modified: Tue, 06 Dec 2022 02:35:14 GMT  
		Size: 58.8 MB (58820449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd665e953b93875afb9c3e029296f59daec9dc6cb87786c91c7dd23abc4ce9f5`  
		Last Modified: Tue, 06 Dec 2022 02:35:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
