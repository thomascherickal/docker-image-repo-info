## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:e57c240bc2c6cc23a0b641b24db04234c07e966bf132ddbc5df82ca9dd253800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:504b1ba00f60e17043bdb95f65f4d8098c8260fa061465e314f0a264f93140af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194816003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a84cfbd926e78c76e91c20aad395cf696099c5ccee5f9dcfb4de97c9859866`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:21:04 GMT
COPY dir:300027169ac55d8fb6f67a0995ca298d5de23ab51f3dc8e227f6e221abd3d2c3 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:21:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:21:04 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:21:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:21:05 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:21:10 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:21:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:21:10 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:21:41 GMT
RUN boot
# Fri, 30 Sep 2022 22:21:41 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b515481e3f48f5ef5749ccfcd2a56e22989feda711462e731a223a16a060f4`  
		Last Modified: Fri, 30 Sep 2022 22:36:08 GMT  
		Size: 103.5 MB (103513866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c0dd459eee6254c2f0c91f0dcd8ec256bc4d70a37dd01651f8b3b3d1a71817`  
		Last Modified: Fri, 30 Sep 2022 22:35:59 GMT  
		Size: 1.1 MB (1077310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ab6e8716c6621eceb1a475d065e212ae873986613d7b53b28a56cf87172bc9`  
		Last Modified: Fri, 30 Sep 2022 22:36:02 GMT  
		Size: 58.8 MB (58820706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9feb54f64441ae110c57afa9cb6003db1ffe58ad2763e7ea641626587ab90b2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.5 MB (192547754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ccc99cdd62064e5672c8bad4b0ba86351442ecabc55ebdbca1fdb3b39115c8`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:41:01 GMT
COPY dir:7668b70c49687fddef57006c57f288afd02ec3ccd6cde9cbc5231ec8fb9225f1 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:41:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:41:02 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:41:03 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:41:04 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:41:10 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:41:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:41:12 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:41:25 GMT
RUN boot
# Fri, 30 Sep 2022 22:41:25 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27700e5297add52eea6aaec46514b5c3aefc9690eb29f23c966f5b6c9a371425`  
		Last Modified: Fri, 30 Sep 2022 23:00:51 GMT  
		Size: 102.6 MB (102613748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf71b369f9fedd637e98af180dadacef2e16023290df29b196e1cc56f465db1`  
		Last Modified: Fri, 30 Sep 2022 23:00:41 GMT  
		Size: 1.1 MB (1064288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96d792cb80b59883366bcf141815023f30a78eefb95973e4dad74ca24bd3162`  
		Last Modified: Fri, 30 Sep 2022 23:00:45 GMT  
		Size: 58.8 MB (58815479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
