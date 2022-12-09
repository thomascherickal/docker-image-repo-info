## `clojure:temurin-8-lein-2.10.0-bullseye`

```console
$ docker pull clojure@sha256:66e7d975c8de34a560f6616dd9de39631f5496f1bd34b153dcdf01f6fb98742c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-lein-2.10.0-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:ce06d488afbfa78bcb47450204b787744fe4e58f57c0407088bca361a10ae04e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176832711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42972a4dd3a025df983c398e3fd9a5ef51000a73b9eae4fe4904806f0f705b6e`
-	Default Command: `["lein","repl"]`

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
# Fri, 09 Dec 2022 22:22:26 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 09 Dec 2022 22:22:26 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 22:22:27 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 22:22:45 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 09 Dec 2022 22:22:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 22:22:46 GMT
ENV LEIN_ROOT=1
# Fri, 09 Dec 2022 22:22:50 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 09 Dec 2022 22:22:51 GMT
CMD ["lein" "repl"]
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
	-	`sha256:0b6b64eaf08f950726e0152b38b6c7171ddc944fc9268386baf199d599f559e7`  
		Last Modified: Fri, 09 Dec 2022 22:43:26 GMT  
		Size: 13.9 MB (13861411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946f4d47f99f01fef13869f488287c7a803d3729de542c28319607439c9c6b81`  
		Last Modified: Fri, 09 Dec 2022 22:43:25 GMT  
		Size: 4.4 MB (4399265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-lein-2.10.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1b2fc25436c698493a1f68d2d5dec8c985b09f6bcd8af0e58ae91607ce28f4f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.6 MB (174574933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cddd16f6b3feeb107258dc4cd7a27763a14c2a4b21b1eab244038fe82dad126`
-	Default Command: `["lein","repl"]`

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
# Fri, 09 Dec 2022 21:39:51 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 09 Dec 2022 21:39:51 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 21:39:51 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 21:40:07 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 09 Dec 2022 21:40:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 21:40:07 GMT
ENV LEIN_ROOT=1
# Fri, 09 Dec 2022 21:40:10 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 09 Dec 2022 21:40:10 GMT
CMD ["lein" "repl"]
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
	-	`sha256:a02852643cf93daf206e575bcf59303104b42a69e6bdd5da2400c5833644c9ac`  
		Last Modified: Fri, 09 Dec 2022 21:48:53 GMT  
		Size: 13.8 MB (13849920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14220c5c90c4813339d2ca7400d4f6e55592c0244fa7b005255574d5d0918820`  
		Last Modified: Fri, 09 Dec 2022 21:48:53 GMT  
		Size: 4.4 MB (4399263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
