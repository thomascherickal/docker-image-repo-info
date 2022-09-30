## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:ede916a58b6f44664322e00b6bfc68147fdd28612ba325d989e16bccf9e6f1f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:05cd5cde2d231ac2bd356342d98a39ed1d72356620288e04229a8b943214aa48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.3 MB (308348985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:900a4ed5099c8fd1c1c3a97cfc5eca04d8e3f8bb80d47487be287290140042cb`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:20:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:27:08 GMT
COPY dir:4a40d0ddbd507a7d3b3a97117be800fbf93534cac954d63629e4fb22f3cd41ad in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:27:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:27:10 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:27:10 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:27:10 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:27:16 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:27:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:27:16 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:27:38 GMT
RUN boot
# Fri, 30 Sep 2022 22:27:38 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:27:38 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:27:38 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0797d39ad88d22b27575060fbd4e4675f49d12e305138f24e08544ecba14490`  
		Last Modified: Fri, 30 Sep 2022 22:39:27 GMT  
		Size: 192.1 MB (192137652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed80a57ce11b40cd6808bdb61f30862792eef55a16aa828dc30837df148e7d`  
		Last Modified: Fri, 30 Sep 2022 22:39:09 GMT  
		Size: 2.4 MB (2360671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a9ded487de12e8b660400af57de5ddfe55cc54d986d3850fb39358faee82b6`  
		Last Modified: Fri, 30 Sep 2022 22:39:12 GMT  
		Size: 58.8 MB (58820528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e38c811c07c9ddb50de8211bb01be360d117a4c2d1f122e52f9ab0dd9265ae`  
		Last Modified: Fri, 30 Sep 2022 22:39:08 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:13389c53b68ef9ecf29e1b1948434ff17505b28fccc241c9afe4d25dd7c5971a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305761078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe3f2a04a8b293bf9ebb2d8ebc03e9b027cde2f8b9831bcebf670f18096f65`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:40:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:47:59 GMT
COPY dir:e8b09aac8a69a5f07df362ceeac55cf5f3321b4ba40e9b02e12250e34b34e83e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:48:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:48:00 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:48:01 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:48:02 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:48:09 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:48:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:48:10 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:48:24 GMT
RUN boot
# Fri, 30 Sep 2022 22:48:26 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:48:26 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:48:27 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ffe5c027f43a0f8dffe3c143fa6c23f9705c59001d637c3093c164b11f8970`  
		Last Modified: Fri, 30 Sep 2022 23:04:37 GMT  
		Size: 190.9 MB (190904318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872f11393d5c2467ba3ac37ee6635506fa49abcea30854ff20ded2e59376e2c2`  
		Last Modified: Fri, 30 Sep 2022 23:04:19 GMT  
		Size: 2.3 MB (2349222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea41b2129228e03b7ca137618b1a753a1000b203f13cd8d494a98435aaecc60d`  
		Last Modified: Fri, 30 Sep 2022 23:04:24 GMT  
		Size: 58.8 MB (58815758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e592a78703a2958eaf0bcda46312ec64d452f17beed979adb99bee8ea65b77d`  
		Last Modified: Fri, 30 Sep 2022 23:04:19 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
