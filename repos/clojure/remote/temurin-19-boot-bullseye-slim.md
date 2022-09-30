## `clojure:temurin-19-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:162bb65b7b8b4daf91af33395961ac6883e7629540a67e5b773fbaf95cd169d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:81377a962ff9070681d6fa521f4ce7ee4ffeb999b671bf30f40363d07a006b55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.1 MB (292146138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486ef249b36314faad6fd5fcae8abc1fdf41f43e9b538359d1ea9a8b0389db91`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:30:53 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:30:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:30:55 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:30:55 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:30:55 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:31:01 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:31:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:31:01 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:31:22 GMT
RUN boot
# Fri, 30 Sep 2022 22:31:23 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:31:23 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:31:23 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bbd00616de1dc5ce1c327c999f5b62b49d54d9d1aecb11cb2cc05bf8fd679d`  
		Last Modified: Fri, 30 Sep 2022 22:41:57 GMT  
		Size: 200.8 MB (200843777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4083f0d6101c91769eac72beb890f909571eb6fd33a953278d5daa86b85011`  
		Last Modified: Fri, 30 Sep 2022 22:41:42 GMT  
		Size: 1.1 MB (1077336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e0de8b6f8ef0e539811435e8696156954f365405053ea107b6224c723628fd`  
		Last Modified: Fri, 30 Sep 2022 22:41:45 GMT  
		Size: 58.8 MB (58820504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee5b6eda029154698bc6843cb6cd88ce234bb009ad364def13e1c3f6132b23`  
		Last Modified: Fri, 30 Sep 2022 22:41:41 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f94bced84eb8417d0e63257e41ba1804c6eeda09821babb05fd7f068e24f1553
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289517382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf6e8c5a5526e37ea7e984aadab25eceb95f2cfb9950a161d8ba30bc9dc3c22`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:52:28 GMT
COPY dir:58f6c37df253d3555e493197f96e3f21593e31d3faf1967e0a7b9d8f0ae9e30c in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:52:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:52:29 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:52:30 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:52:31 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:52:37 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:52:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:52:39 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:52:52 GMT
RUN boot
# Fri, 30 Sep 2022 22:52:54 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:52:54 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:52:55 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e88c33693f932839a1b6d9254e2e1ad8799153952e412da2891fa1679ec8b`  
		Last Modified: Fri, 30 Sep 2022 23:07:34 GMT  
		Size: 199.6 MB (199582874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6eea4197dcec1633f8a78b8cabfc4e7b5aaf4fe826a4fde382c8d89a052866`  
		Last Modified: Fri, 30 Sep 2022 23:07:15 GMT  
		Size: 1.1 MB (1064295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74865f24f460e41b095c614a61693983255a82341175cfabceddd312c15fce6`  
		Last Modified: Fri, 30 Sep 2022 23:07:21 GMT  
		Size: 58.8 MB (58815573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c5a716219e192335efa5d47661cb4a29a3b2023c6af2c4586c427f0d801825`  
		Last Modified: Fri, 30 Sep 2022 23:07:15 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
