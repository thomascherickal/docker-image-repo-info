## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:8e47acf5946cc86a9cee68f16463ee3b30ebb6db514931f9809b2103ebf73ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b81080409191674c653f1b451f3160b737239ba1cf7cea2b5e039e46779e3197
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.7 MB (289749328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57c3b8dc2059f192a4601a0b03409b3282d28a9fc01dc60b4471aa63fc5371ef`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:51:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:54:03 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:54:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:54:05 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 01:54:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 01:54:05 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:54:11 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 01:54:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 01:54:11 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 01:54:30 GMT
RUN boot
# Wed, 21 Dec 2022 01:54:30 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6db9c94a4957a1754107e38ff03b70c980e609a9f349a218009678a8917b1b7`  
		Last Modified: Wed, 21 Dec 2022 02:07:20 GMT  
		Size: 198.5 MB (198454552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5283604d8de6a9106851812fd34d45e511819ba968a783e1e5f50788c461ee67`  
		Last Modified: Wed, 21 Dec 2022 02:07:05 GMT  
		Size: 1.1 MB (1077338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98874b25a34a3aea6622817e5da7b1810c464f2fa525fb48400fd1d89ab9942d`  
		Last Modified: Wed, 21 Dec 2022 02:07:08 GMT  
		Size: 58.8 MB (58820495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1e1e0fc18c12472895d4ff5891b678bf60e95287b642e6201e6dd72d8416fd20
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.1 MB (285133245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbc708935eed0a354c6d4605a8b05535df90db5d3245130533924bd88127449b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:21:14 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:21:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:21:18 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:21:19 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:21:19 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:21:23 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:21:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:21:23 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:21:40 GMT
RUN boot
# Wed, 21 Dec 2022 02:21:41 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418e472fbc1e675c21a46f7fc728e7299e4becc0622adce50ed53160c548c7f0`  
		Last Modified: Wed, 21 Dec 2022 02:32:36 GMT  
		Size: 195.2 MB (195203361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb0fe455b7d8351e96da19719664db6577a60169a88307ebd33dc9b5e8a5b12`  
		Last Modified: Wed, 21 Dec 2022 02:32:25 GMT  
		Size: 1.1 MB (1064618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09503437f1b3bc565d19ba86fc7cd8722951bf564b05c0f4697a1c67351a9844`  
		Last Modified: Wed, 21 Dec 2022 02:32:28 GMT  
		Size: 58.8 MB (58820494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
