## `clojure:temurin-11-lein-2.10.0-bullseye-slim`

```console
$ docker pull clojure@sha256:0e320d5c93e6cfd3d8fe2d503cf985f4babc50766490e49fe28593aebe58420b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.10.0-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a047b0aa7bedc752dfc636edf97f755604b1033d35b9df67e8ee034b201e72aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246928522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc94ef71ccb31c2338f521f34c2e7d1f30c70dbe86040bf216cd5e035c4bbc2`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:55:29 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Thu, 04 May 2023 14:55:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 14:57:00 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 04 May 2023 14:57:00 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 04 May 2023 14:57:00 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:27:45 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 19 May 2023 20:27:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 19 May 2023 20:27:45 GMT
ENV LEIN_ROOT=1
# Fri, 19 May 2023 20:27:49 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 19 May 2023 20:27:49 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8debf5f3c7bd7d820f2797f8d4cfc95b7902d0071ca115228b3f6eb2d872a`  
		Last Modified: Thu, 04 May 2023 15:06:32 GMT  
		Size: 198.5 MB (198549506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b698d10c33d86d19fca98b1d49d57e0b74a34df08c9d15c7f115da41971937`  
		Last Modified: Fri, 19 May 2023 20:39:03 GMT  
		Size: 12.6 MB (12576258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bd5aba1be728d918ef3909dcaba2b87c5dd66e57de4619ea01454278d3a24`  
		Last Modified: Fri, 19 May 2023 20:39:02 GMT  
		Size: 4.4 MB (4399242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.10.0-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:edee20b2e3930a7b56861357b0a9c7eb99aa6e9ce7a35152bb44467eaea394fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242339895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91263bcc2de059625e58aaace8438e8832eafe5d789cdcb3165f1190ef71f621`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:27:27 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Tue, 23 May 2023 01:27:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:28:21 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 23 May 2023 01:28:21 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:28:21 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:28:34 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 23 May 2023 01:28:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:28:35 GMT
ENV LEIN_ROOT=1
# Tue, 23 May 2023 01:28:37 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 23 May 2023 01:28:37 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78c86840ae584aab4d9f49c5158125ceb03a9fcfcbb243c03ce4819b42d8729`  
		Last Modified: Tue, 23 May 2023 01:35:49 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7a411681312c318f27c1ed2c2a7115bb80dd3af4ac16c5d2f307c0777fddeb`  
		Last Modified: Tue, 23 May 2023 01:36:09 GMT  
		Size: 12.6 MB (12563665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a60bfc7fe357a89706477995f11bb8cd5c54d47e579b4c29b9ad50101f30f`  
		Last Modified: Tue, 23 May 2023 01:36:08 GMT  
		Size: 4.4 MB (4399274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
