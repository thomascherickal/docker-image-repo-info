## `clojure:temurin-8-tools-deps-1.11.1.1200-bullseye`

```console
$ docker pull clojure@sha256:e0b5b0b96d701f4d239f832ed4e36323895d4bcb6c374a1c4bb995ecd3bde2b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1200-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:9ebad960f6e6851b502cff4b7dc51fa5a958c59150ccc0c8ebe2e47254785ea2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205884037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f131c596d91b75ffba258169fd2f6823d9ac3f510257a06ad29e7bbfb17b891b`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:48:45 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:48:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:50:51 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 01:50:51 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:51:07 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 01:51:08 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 01:51:08 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d55e2e180666cd09635874932249e6b38c8a236bbe474c85aeeaf3a3e9c48c2`  
		Last Modified: Tue, 06 Dec 2022 02:03:18 GMT  
		Size: 103.5 MB (103530693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aeba4973278bdee0901c1a72696defde5b3ebcaabdab3ad05a781db306890`  
		Last Modified: Tue, 06 Dec 2022 02:04:19 GMT  
		Size: 47.3 MB (47311385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bdc50dc42c0015d6130ed43e054a385007e0b0637dcd7c0c3a0d9f6bd2fcf2`  
		Last Modified: Tue, 06 Dec 2022 02:04:13 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-1.11.1.1200-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:36ee16d1570c8333d50eeb86dea060daa10c7188d18f3c4918a57c663f15ed89
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203630668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caa89aadc4c73598f425ee5e9f23f4ae83121590acc8fd2900142204952a8f4`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:17:16 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:17:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:19:05 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 02:19:05 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:19:18 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:19:18 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:19:18 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f371d9828c94870641f3c611f4a9fda6d693a78baa752a2efcea3cab5826d80`  
		Last Modified: Tue, 06 Dec 2022 02:29:56 GMT  
		Size: 102.6 MB (102626604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5c1eab78e9769073d21c829f43f0e126a7cb39a1addf7eeb184ed509e4d5c`  
		Last Modified: Tue, 06 Dec 2022 02:30:50 GMT  
		Size: 47.3 MB (47304300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c472305b468838c6e2e0bdc56ef2dc8df33a1b33f8e79edfcda7e6ea8a67e6d`  
		Last Modified: Tue, 06 Dec 2022 02:30:45 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
