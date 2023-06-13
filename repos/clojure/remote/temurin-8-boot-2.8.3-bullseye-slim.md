## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:82289510fdb41bc66740cca82cc4a138e58ae6e939a6547a2bc94a0d68ce1b37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:83c509b8fc6bed073eb3913795556a6ec511602acc31bc24599bec80dca2a31f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.0 MB (145957654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca2a236faf7560c8e084ac5417f09096528432fa4c60eaec4a144dbfeb3e0ed`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:44:38 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:44:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:44:38 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:44:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:44:38 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:44:44 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:44:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:44:44 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:45:04 GMT
RUN boot
# Tue, 13 Jun 2023 03:45:04 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a06b2482c1581bf48768b9037153a524f6626b4fdbab3333e123405ee98c4d`  
		Last Modified: Tue, 13 Jun 2023 03:55:36 GMT  
		Size: 54.6 MB (54642102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70be3158a98adeb47fc61efc83b7dcd346740355508515d5f8109db2e09a21`  
		Last Modified: Tue, 13 Jun 2023 03:55:30 GMT  
		Size: 1.1 MB (1077509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa0a26ad0b8d03d61ba1be2a97ecec908d8b71ebdbc54067d88b001876ceb61`  
		Last Modified: Tue, 13 Jun 2023 03:55:33 GMT  
		Size: 58.8 MB (58820633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c0121184129b872dcd44625b9b28fdac630b3414f13128483c76a577d72846ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143690826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4feb9b38699c2da5e6ccba3bc24031e0595af74d871e6e72780296616f61b650`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:51:12 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:51:14 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 04:51:14 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 04:51:14 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:51:19 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 04:51:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 04:51:19 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 04:51:38 GMT
RUN boot
# Tue, 13 Jun 2023 04:51:38 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c42dbe9973fad0e5db82fff74ab48ee24033b2296cd2ca6fdcba69bad893d2`  
		Last Modified: Tue, 13 Jun 2023 05:00:32 GMT  
		Size: 53.7 MB (53742662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb9b6fcda3aedb785b8140b3f436e957c38f2432ef3105ba11c8c424ad63e8c`  
		Last Modified: Tue, 13 Jun 2023 05:00:28 GMT  
		Size: 1.1 MB (1064827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f65ac90055caa13ed11c5ea58aaa9733282740c60dce501ac500e80018950`  
		Last Modified: Tue, 13 Jun 2023 05:00:30 GMT  
		Size: 58.8 MB (58820503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
