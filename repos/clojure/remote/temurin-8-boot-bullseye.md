## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:5a6a403c0983bc8b1b2981ba2dc620829881629176821c70a3b98ffd1e825c30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:df74cf07eb4dfaf646f93d70970985632154d33e467f1b39a012a3ea590d30bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219725363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12471a2c31ed2f524bcd6e2bac1c59ffe92cabb6b2d313d47e300a42f9d0d980`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:20:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:20:07 GMT
COPY dir:300027169ac55d8fb6f67a0995ca298d5de23ab51f3dc8e227f6e221abd3d2c3 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:20:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:20:08 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:20:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:20:08 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:20:15 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:20:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:20:16 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:20:58 GMT
RUN boot
# Fri, 30 Sep 2022 22:20:58 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59c6809a4902ba9e9419a0a914f03fb8a79a99989580f9a589a14256bf1122b`  
		Last Modified: Fri, 30 Sep 2022 22:35:49 GMT  
		Size: 103.5 MB (103513858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cce2820be13b0611f50ea8c0169f692a2847ed236dcefe03b0f63c6a1bfe31`  
		Last Modified: Fri, 30 Sep 2022 22:35:41 GMT  
		Size: 2.4 MB (2360780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1580c25575901e7375c6a6dc7b326af3b0ba8d5c2a07cc14631f350a9e1b492c`  
		Last Modified: Fri, 30 Sep 2022 22:35:44 GMT  
		Size: 58.8 MB (58820993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0d5cd3af69bfccf8aeb29eb50839abf18237f86ddf3de4c9a643e7630272fa2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217470174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62b67bc96088ab7ee78a2e87994d7c28bdf9c14c7cf7774364181ef6c99a3ed`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:40:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:40:24 GMT
COPY dir:7668b70c49687fddef57006c57f288afd02ec3ccd6cde9cbc5231ec8fb9225f1 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:40:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:40:25 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:40:26 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:40:27 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:40:34 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:40:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:40:36 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:40:52 GMT
RUN boot
# Fri, 30 Sep 2022 22:40:52 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb22d2091400e568eee0541108b6f129859dc7241712d7e566660b3bf86e2bae`  
		Last Modified: Fri, 30 Sep 2022 23:00:30 GMT  
		Size: 102.6 MB (102613747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ec00e8c0a405a5d1a6fd4de7872fcf5b6e09f888a22ce4bef8f838db1afdb`  
		Last Modified: Fri, 30 Sep 2022 23:00:20 GMT  
		Size: 2.3 MB (2349296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a798cc3a70d8f1a9a045a5da9f94e299c1f02c3587f35586569e7fa5fec5c523`  
		Last Modified: Fri, 30 Sep 2022 23:00:26 GMT  
		Size: 58.8 MB (58815751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
