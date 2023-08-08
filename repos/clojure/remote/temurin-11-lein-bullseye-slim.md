## `clojure:temurin-11-lein-bullseye-slim`

```console
$ docker pull clojure@sha256:63456e3ef38cd933c9f69941f322de3bbd9b0736428c528c10583cd9762ceed3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:53e46ac8e3f4dc12b6ad77c237026dd7a2c164ca3f3012a696e6ce2d90d5a4e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193222766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0524d99f9972dc0040308551974d2eb4d7c10bcee372d07d8cd7da5e3732f84`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:22:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 02:22:57 GMT
COPY dir:2fc258758bb2c25982e4c8348cffe5a1ab54f4c54e52ff852a817cdf5bd62215 in /opt/java/openjdk 
# Fri, 28 Jul 2023 03:17:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 03:18:30 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 28 Jul 2023 03:18:30 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 28 Jul 2023 03:18:30 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 03:18:44 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 28 Jul 2023 03:18:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 28 Jul 2023 03:18:44 GMT
ENV LEIN_ROOT=1
# Fri, 28 Jul 2023 03:18:47 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 28 Jul 2023 03:18:47 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8093463543ce0d2e4cc72a5011db04a63e89f8a49c37702622adc8e1defc155b`  
		Last Modified: Fri, 28 Jul 2023 02:25:48 GMT  
		Size: 144.8 MB (144829555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f472b62e2d3ac502e1576492efb0dd269a4d262cea757c8bc27ab57e4fd627`  
		Last Modified: Fri, 28 Jul 2023 03:30:17 GMT  
		Size: 12.6 MB (12576328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cfe9f8f7835c2970f6502e68508e11cc1d135a855909b0666ed967b02e32fa6`  
		Last Modified: Fri, 28 Jul 2023 03:30:17 GMT  
		Size: 4.4 MB (4399281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:156dc5b544cbc9833ae1436549a6df998aa6239facacfaf6f20aa0c04c92f63a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.6 MB (188591163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4a620401b74ad3a200a1453853b3782bc6cb7877c459c83035e7d1841926eb`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:25:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:21:30 GMT
COPY dir:ddfd64e7bd36f630cd100cf454a9685f9fd0f9483467dbf7a4c9a71ab0af7089 in /opt/java/openjdk 
# Tue, 08 Aug 2023 20:21:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:23:09 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 08 Aug 2023 20:23:09 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 20:23:09 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 20:25:34 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 08 Aug 2023 20:25:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 20:25:34 GMT
ENV LEIN_ROOT=1
# Tue, 08 Aug 2023 20:25:36 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 08 Aug 2023 20:25:36 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4618d52dbf5263b6400122ab8ead6b84fd0a5fdd684ed03f8e4a606dff09c08e`  
		Last Modified: Tue, 08 Aug 2023 20:32:48 GMT  
		Size: 141.6 MB (141565379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d24f402580e98bf54fa9912b271581356c3c9be308fb77837011ccb6605c106`  
		Last Modified: Tue, 08 Aug 2023 20:33:38 GMT  
		Size: 12.6 MB (12563700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb85d3c85d2675cb61503e60c0a9b4e5b04b009d7469437b1f6d9506aabdbc9`  
		Last Modified: Tue, 08 Aug 2023 20:33:38 GMT  
		Size: 4.4 MB (4399253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
