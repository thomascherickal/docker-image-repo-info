## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:729789c222ab973d59e8ee5e774b8c9b9c8736a315450fa72c340f875db8a8cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:21fd8726754b12597d99d73b950d6e417991f1d6c24c2f1159b21b634f0e8689
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.4 MB (289444431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5247bcea56f34b7464b02c53fe4e1c9f72ad5a62b4da60217be7dc6a1b582e7`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:36:56 GMT
COPY dir:e3c63d67b32fccda756dd62000a0cf47da966d18fe6f1f25cd1f37b60881f0ec in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:36:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:36:58 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 25 Oct 2022 02:36:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:36:58 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:37:04 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 25 Oct 2022 02:37:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:37:04 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 25 Oct 2022 02:37:26 GMT
RUN boot
# Tue, 25 Oct 2022 02:37:26 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baa79e738b7c5239823844cc2dde0b88b3b0c50dc1863902d1c9a329b737a80`  
		Last Modified: Tue, 25 Oct 2022 02:50:28 GMT  
		Size: 198.1 MB (198124970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441847100f9aa58f97eea058eac0f8063dbc1992f6f65f47a3b360dc10ba520d`  
		Last Modified: Tue, 25 Oct 2022 02:50:14 GMT  
		Size: 1.1 MB (1078964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4e6ad4da7bd7a938c2e31c1b035d2be9f6d1cde2f529f807c528639a44b463`  
		Last Modified: Tue, 25 Oct 2022 02:50:17 GMT  
		Size: 58.8 MB (58820459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:156b1128238223d87e83562f5d807419f30e1b262b1e2aada48c6bbf26649d06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.8 MB (284817691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee18e267e89b155b19e41efed3f3ac5faf3a1450f66a9e38263c94dcf0eccac`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:38:30 GMT
COPY dir:0c9c8c2b9cd43799d246d5824c591352650ad79f5d15544287f00c2deb1e4608 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:38:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:38:34 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 15:38:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:38:35 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:38:39 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:38:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:38:40 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 15:39:05 GMT
RUN boot
# Wed, 26 Oct 2022 15:39:05 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3d7b35da3e357173d5404cc59df1a4394d6031ee4598b02de7918d2110bae`  
		Last Modified: Wed, 26 Oct 2022 15:58:03 GMT  
		Size: 194.9 MB (194866982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8efba58aed44cfe3eb1a9353e28bcc19d18fea23eb89deaee04bf4ad23b32d`  
		Last Modified: Wed, 26 Oct 2022 15:57:52 GMT  
		Size: 1.1 MB (1066323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f125baacd294c02c41c4afa3b7484f5f462c20f146ca4e02562d4b56f137da`  
		Last Modified: Wed, 26 Oct 2022 15:57:54 GMT  
		Size: 58.8 MB (58820476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
