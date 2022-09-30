## `clojure:temurin-17-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:72bdff935faefea279f5b559399e196fc1437ea9c12c05372dfbfea9faef08ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:cd09d0edcfe3139b15b143dff4ca9aaf5a8a9766ce86ef9106eb779337fe20e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.4 MB (283439849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff27f42c233e92827e2fed513d80282b25d049208cf36c95de42c3afd80cd8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:27:47 GMT
COPY dir:4a40d0ddbd507a7d3b3a97117be800fbf93534cac954d63629e4fb22f3cd41ad in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:27:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:27:48 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:27:48 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:27:48 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:27:54 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:27:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:27:54 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:28:14 GMT
RUN boot
# Fri, 30 Sep 2022 22:28:15 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:28:15 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:28:15 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65a48fb445eb8f9528419bdb749aff629072fae69a78a509e2773ba76d43379`  
		Last Modified: Fri, 30 Sep 2022 22:39:51 GMT  
		Size: 192.1 MB (192137446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07487a177621dfcdf88dfe540b06f8ac74ce80d9e154027ac16c7d5f0c69dc`  
		Last Modified: Fri, 30 Sep 2022 22:39:37 GMT  
		Size: 1.1 MB (1077293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d0952f8b913f1ecd07adee88ebeae2cdbed49058aa28eeb1b5fdbb894db420`  
		Last Modified: Fri, 30 Sep 2022 22:39:40 GMT  
		Size: 58.8 MB (58820588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c08a6f651c98b4b0f61bfe521762f015ff361f1f7478e5a838223de9d57d116`  
		Last Modified: Fri, 30 Sep 2022 22:39:36 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:33f538cdde9cb2a722a2ae8f094a3e3439a19a5a9571b111a8cc15dc7ee4f98a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.8 MB (280839234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf2c22e72af194b9c22e3f2178289500f865b315b1ce8200e82b76f3ab63438`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:48:36 GMT
COPY dir:e8b09aac8a69a5f07df362ceeac55cf5f3321b4ba40e9b02e12250e34b34e83e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:48:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:48:37 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:48:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:48:39 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:48:45 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:48:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:48:47 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:49:01 GMT
RUN boot
# Fri, 30 Sep 2022 22:49:03 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:49:03 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:49:04 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e9ee07116b1c34e53212577545c764c310f4ad2784f78e99382d4f859d340`  
		Last Modified: Fri, 30 Sep 2022 23:05:05 GMT  
		Size: 190.9 MB (190904320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b8c903b1de8d4db9cf538fa9309297dc050cfd581afe0014d045a097a27366`  
		Last Modified: Fri, 30 Sep 2022 23:04:49 GMT  
		Size: 1.1 MB (1064304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e051888cc5350ba46dc8ec7f674d5f0086e900063554797f1eabed5433c46618`  
		Last Modified: Fri, 30 Sep 2022 23:04:53 GMT  
		Size: 58.8 MB (58815971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9738ca93fe9cd8eba0d91f8750e58cd14c2afbcd093374715f1d56388bda62`  
		Last Modified: Fri, 30 Sep 2022 23:04:49 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
