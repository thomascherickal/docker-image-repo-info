## `clojure:temurin-11-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:87170ebd7b33b2941ff657867699c02b7e3a78fbc895ce51c753e03a367fd025
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:814ba745a58acec2b2e32fcbea488063ce78e8b0ea904f0809874e9e70e8f8ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289865158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbea70a22200df1bb61d7d4c890265f8b88dc276932b2420e797ec7f79474736`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:47:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:47:31 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 03:47:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:47:31 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:47:36 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 03:47:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:47:36 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 03:47:54 GMT
RUN boot
# Tue, 13 Jun 2023 03:47:54 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896461db9dc8d8ddae7e64687a1ce367f7d901f4479b693b57f1d1db44f9bf49`  
		Last Modified: Tue, 13 Jun 2023 03:57:10 GMT  
		Size: 1.1 MB (1077537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e34c439c42ec7516b8fc62c481bf9cf867848409c4d1df967fc44545b0f6d9c`  
		Last Modified: Tue, 13 Jun 2023 03:57:13 GMT  
		Size: 58.8 MB (58820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5b493dd31e4660800657d5109e5550c126d5c270774f567ac54d9e6d9ea6ea0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285272497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f512c8e8bee1f82cfe6a5331fe00f4f2980c2187e7338418ce427b0c45d947`
-	Default Command: `["boot","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:29:47 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:53:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:53:42 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 13 Jun 2023 04:53:42 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 04:53:42 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:53:46 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 13 Jun 2023 04:53:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 04:53:47 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 13 Jun 2023 04:54:04 GMT
RUN boot
# Tue, 13 Jun 2023 04:54:05 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c7296223cd8d65203506b7cc022a934e2af6937394ef0f20e9a9d29a67dc4`  
		Last Modified: Tue, 13 Jun 2023 04:31:52 GMT  
		Size: 195.3 MB (195324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7295a78d6a6d221f0590e2647b7e341c223ad1252fdfefb7748d60bb354ca3b`  
		Last Modified: Tue, 13 Jun 2023 05:01:56 GMT  
		Size: 1.1 MB (1064846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5da4405a5f21ad6adabd6227587a93d8c6f81e088cf2984cc6b5415c52f19e3`  
		Last Modified: Tue, 13 Jun 2023 05:01:59 GMT  
		Size: 58.8 MB (58820605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
