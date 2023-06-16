## `clojure:temurin-11-lein-2.10.0-bullseye-slim`

```console
$ docker pull clojure@sha256:3c24c9d01d2bc3c830f1747f56ddb0fb707cc0a6b87dc074d71e2c5824b2cfd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.10.0-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:dcc33e963fdac6a11fe519aa1e13cce78d00552c4b6817eee51437a798d0d040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246942661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7d7436ae74cdb5ec470976922beefae99ccb154af788226aeb3903c9ade87a`
-	Default Command: `["lein","repl"]`

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
# Tue, 13 Jun 2023 03:48:28 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 13 Jun 2023 03:48:28 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:48:28 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:48:42 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 13 Jun 2023 03:48:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:48:42 GMT
ENV LEIN_ROOT=1
# Tue, 13 Jun 2023 03:48:45 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 13 Jun 2023 03:48:45 GMT
CMD ["lein" "repl"]
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
	-	`sha256:62f8b7e02c08074cbeb85746c7b1cf1e229fa9f911818cb2b4177f7efc821c61`  
		Last Modified: Tue, 13 Jun 2023 03:57:43 GMT  
		Size: 12.6 MB (12576272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580b81c15a42f469eca5c27dffa624e32cff16794f687a1f0d04defa51296ed5`  
		Last Modified: Tue, 13 Jun 2023 03:57:43 GMT  
		Size: 4.4 MB (4399285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.10.0-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a57c2c33094e723499ba620d6e219b991feb5c89ecb8f69d8eadbf581e9425ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242349926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97016287695bb92985a1a43c37b1fbffd5752cd34cc01c627800daa8428132f0`
-	Default Command: `["lein","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 04:42:21 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Fri, 16 Jun 2023 04:42:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:44:12 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 16 Jun 2023 04:44:12 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 16 Jun 2023 04:44:12 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:44:25 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 16 Jun 2023 04:44:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 16 Jun 2023 04:44:25 GMT
ENV LEIN_ROOT=1
# Fri, 16 Jun 2023 04:44:28 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 16 Jun 2023 04:44:28 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f561dc152f6d05a1820783d780247855889a7f67c10ad93e662c845bc4e04b7`  
		Last Modified: Fri, 16 Jun 2023 04:54:22 GMT  
		Size: 195.3 MB (195324188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb72c4bf93853a9fc8f020324881cfceaa5f814299c3ea9198fa6b38eb9eb80`  
		Last Modified: Fri, 16 Jun 2023 04:55:11 GMT  
		Size: 12.6 MB (12563695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7629858449b20bdcd6009c48117d61d80f3d0d76b6c38b17fb0d137e79963949`  
		Last Modified: Fri, 16 Jun 2023 04:55:10 GMT  
		Size: 4.4 MB (4399209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
