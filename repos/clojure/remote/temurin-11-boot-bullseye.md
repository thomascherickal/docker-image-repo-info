## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:e58547aaa59bc41cc7bc29c33160d204800d6967a3d8c5e197dc865437b49421
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:5726c90f3784edf609c31865ad35fb9f8ce935746bc20f733d870e1a9d581214
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314661084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a287aae45894a907a37e2e6060cb60d71fccbd854d93b67829c7663df6acfd20`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:53:31 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:53:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:53:32 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 01:53:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 01:53:33 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:53:38 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 01:53:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 01:53:39 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 01:53:57 GMT
RUN boot
# Wed, 21 Dec 2022 01:53:57 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09879893307507e7fe968e99bda720fc4263e5da6b74edf0064ca1f992ab9605`  
		Last Modified: Wed, 21 Dec 2022 02:06:55 GMT  
		Size: 198.5 MB (198454573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40919b3b9da0bda0e8aef511927e9e2a2fbb0b81559ec8887f8f142409c73825`  
		Last Modified: Wed, 21 Dec 2022 02:06:41 GMT  
		Size: 2.4 MB (2360765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91978998a5b59a7615b6848be8262477c4b52c48533797affbe91c0a40cf8290`  
		Last Modified: Wed, 21 Dec 2022 02:06:44 GMT  
		Size: 58.8 MB (58820580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0d880efb3232fc07af85c23f3abe4fb9bcea8f61a8ac091e09fb9287d71e8491
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310056325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:655a057b8c2585d669df644742dde3433bca8b5b5c9052a6c4c79df6d5d31ac4`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:20:42 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:20:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:20:46 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:20:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:20:46 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:20:51 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:20:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:20:51 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:21:08 GMT
RUN boot
# Wed, 21 Dec 2022 02:21:09 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba82789481f43d21d6d2ece93afb47a4345ba46f2c082c71dcc84a5ef12fb90`  
		Last Modified: Wed, 21 Dec 2022 02:32:16 GMT  
		Size: 195.2 MB (195203346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1aa24bcae2156d352da826c8ded48dedd54598f21651cd82b6707e1f3ea43b0`  
		Last Modified: Wed, 21 Dec 2022 02:32:05 GMT  
		Size: 2.4 MB (2350614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105511176343f641a786ee17ac543409065ca38f5a07af7ed8e2c92e05c3931d`  
		Last Modified: Wed, 21 Dec 2022 02:32:08 GMT  
		Size: 58.8 MB (58820568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
