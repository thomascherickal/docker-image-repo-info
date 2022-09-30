## `clojure:temurin-11-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:31e76006b94079272e24b3d81c370eb4c56caad625a75efd2c16cfdbc310ad84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:5938b8b5a2b71f9947d22231001ec1abe3120f971490a08016722c8cdcdc90fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.3 MB (314335936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639ef1b8ef3ee5945c0abf7e7570b118172b047df7cccfc5c45a0005f0e146f4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:20:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:23:55 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:23:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:23:57 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:23:57 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:23:57 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:24:03 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:24:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:24:03 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:24:30 GMT
RUN boot
# Fri, 30 Sep 2022 22:24:30 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9489cf708b9c57f6b8585996c4aef3fd0dffac96db31dce0b646256dfd6607`  
		Last Modified: Fri, 30 Sep 2022 22:37:39 GMT  
		Size: 198.1 MB (198124868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851dbb798f49c54a52c76fd027353255b2ba4bdd7c2832ff7d5bad2713453846`  
		Last Modified: Fri, 30 Sep 2022 22:37:24 GMT  
		Size: 2.4 MB (2360750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568ef645acfd95e344e4c7c11ded56e7dae90ecbdeecc86a6cc01aae7277e4f`  
		Last Modified: Fri, 30 Sep 2022 22:37:28 GMT  
		Size: 58.8 MB (58820586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:844c55257901310fcbdd7d16830b0c188a6bba5cfee0acc2124c06373b80d81c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.7 MB (309724155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca3056837a5b90e983ad46581a627750e465cad6cdb16a7a459f070ed409a70`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:40:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:44:15 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:44:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:44:17 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:44:18 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:44:19 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:44:26 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:44:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:44:27 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:44:42 GMT
RUN boot
# Fri, 30 Sep 2022 22:44:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496229bd9bf2839e6a37383e68eb8152323866be978a27514af1c0315606d266`  
		Last Modified: Fri, 30 Sep 2022 23:02:36 GMT  
		Size: 194.9 MB (194867813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a28b5a8c3c0deda259057f6e2ffa83fe23b856e1898d355edb35e1ad92acf31`  
		Last Modified: Fri, 30 Sep 2022 23:02:18 GMT  
		Size: 2.3 MB (2349264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0b6deec3c16b01fda61ce207aa511e9a9fca225dfca56e604db1810310ff35`  
		Last Modified: Fri, 30 Sep 2022 23:02:24 GMT  
		Size: 58.8 MB (58815698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
