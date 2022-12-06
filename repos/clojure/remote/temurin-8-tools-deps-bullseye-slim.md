## `clojure:temurin-8-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:91fe392d563ba7b4d55b76e3d399069b20fd5f6a9d2643b4f5927ff614d3f25b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:8b34b1b32f4a29a01f9bd7018e164b106fc051bce495950c86dc9b0240b96f6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196428627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d04139265d368dbbc227e80936e1625a93418621a1b9a4b31bb35c17fe70c4`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:49:18 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:49:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:51:11 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 01:51:11 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:51:30 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 01:51:31 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 01:51:31 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4affc3cd73f667de2263e106409ed3d854f8bd2cd76ecd0a5e3aca312c862bff`  
		Last Modified: Tue, 06 Dec 2022 02:03:39 GMT  
		Size: 103.5 MB (103530647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52de7750f146de49f31d312d6cbf04c4e27313aa4148071822b52a4eecccaa33`  
		Last Modified: Tue, 06 Dec 2022 02:04:37 GMT  
		Size: 61.5 MB (61484510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c44ea1fdb94ef8e5b4440c01766585e7a243aa454370945356ef25e97b9ed`  
		Last Modified: Tue, 06 Dec 2022 02:04:29 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:02e4c6ab966425ba6dd8278deeafd2b3004169db7e1e321b63147d8abaf3cad9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194291772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac06f0d72f37e50a064c73f4161d8f9c08000907055cd716f1b798815e1e4af7`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:17:49 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:17:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:19:22 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 02:19:22 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:19:36 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:19:36 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:19:36 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5df8fef8a794006d98d0afa5f4cd031bef7bb0b991129e393fd59e5565be509`  
		Last Modified: Tue, 06 Dec 2022 02:30:13 GMT  
		Size: 102.6 MB (102626601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860f490855809990242d97a2aa2ca09b005e3345c25bca32319910a26a55dee6`  
		Last Modified: Tue, 06 Dec 2022 02:31:06 GMT  
		Size: 61.6 MB (61604234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57e0c2ba64a753efd752e2475231e1833479f7b5f3dfbe6e677b5fab54b97f7`  
		Last Modified: Tue, 06 Dec 2022 02:31:00 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
