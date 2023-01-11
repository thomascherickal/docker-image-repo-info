## `clojure:temurin-19-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:9feb085e2f2af986e3307f20c8e18947431d1f2dd4eb2d1d52add57d4a8b3dae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:8582bd45e27f332f393ba18cc7eb7b705a86a03b516ca58c1a6abcf521586b95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292398691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf3eaecf54ff6ea454ee0fb979db9266b7d5e5b4aa92a20d4e7a76b68df32c85`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:29:24 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:29:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:29:25 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:29:26 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:29:26 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:29:31 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:29:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:29:32 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:29:51 GMT
RUN boot
# Wed, 11 Jan 2023 03:29:52 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:29:52 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:29:52 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d8be54a6a27b2dcfcf7bef696c11a2997b5312abc571cedd943a85c4d8dbea`  
		Last Modified: Wed, 11 Jan 2023 03:40:45 GMT  
		Size: 201.1 MB (201103413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cd1f4f4c2d19713b0485e9b6816500b84e2ec42a577897c42177df60fddcb7`  
		Last Modified: Wed, 11 Jan 2023 03:40:30 GMT  
		Size: 1.1 MB (1077328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3802ce5cd5490802b01861d562884ce35719dd28cc13fcda5f5a993857c28809`  
		Last Modified: Wed, 11 Jan 2023 03:40:33 GMT  
		Size: 58.8 MB (58820579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c825c32c50bef5f1d6c6154a1cc3bc2bf1e7def5b698bc1a39b399370d0a21f0`  
		Last Modified: Wed, 11 Jan 2023 03:40:29 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:730c3199df9276671bb4fcdbd7542e300dfb9801e442ae169eb666773bf6c813
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289794770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b2a61b2a00717fb66b946fc77454d796bfc5c9d7d76a01dca0e9fdf05d06bd`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:46:26 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:46:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:46:31 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:46:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:46:31 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:46:36 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:46:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:46:36 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:46:53 GMT
RUN boot
# Wed, 11 Jan 2023 03:46:54 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:46:54 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:46:54 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa89f4fc9f09a63d5cbae62dce013f90ebadeb7676212824b1c3bb4ea7e3cbc`  
		Last Modified: Wed, 11 Jan 2023 03:56:25 GMT  
		Size: 199.9 MB (199864415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4802d3ebc491ff5a48bbd20c93e672d8a5c298dfd92e565405f9e5aec0ddc623`  
		Last Modified: Wed, 11 Jan 2023 03:56:12 GMT  
		Size: 1.1 MB (1064665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c90699c372eb385b31dce7d0aa3781fc553d2250b37638100c4f3a18ca0d45e`  
		Last Modified: Wed, 11 Jan 2023 03:56:15 GMT  
		Size: 58.8 MB (58820478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6923f1ab295b5a164da63c8fca12f678774466e288bc1798c9c4dd41b38d9eb3`  
		Last Modified: Wed, 11 Jan 2023 03:56:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
