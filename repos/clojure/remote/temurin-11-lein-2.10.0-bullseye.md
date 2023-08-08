## `clojure:temurin-11-lein-2.10.0-bullseye`

```console
$ docker pull clojure@sha256:f26771f1ad7abba66ad461e1e030da608c6bf99aee209f007d7bd6531ba867bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.10.0-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:1bcdd44467720246a7a78d145831203bc864b48e06590969b5f3339e7aaacebc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.1 MB (218145700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d183cfce12629ab2533e38a964411aa7181a2f3777b8e396146ae8975a3b3e1`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 03:17:02 GMT
COPY dir:2fc258758bb2c25982e4c8348cffe5a1ab54f4c54e52ff852a817cdf5bd62215 in /opt/java/openjdk 
# Fri, 28 Jul 2023 03:17:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 03:18:10 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 28 Jul 2023 03:18:10 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 28 Jul 2023 03:18:10 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 03:18:24 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 28 Jul 2023 03:18:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 28 Jul 2023 03:18:24 GMT
ENV LEIN_ROOT=1
# Fri, 28 Jul 2023 03:18:27 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 28 Jul 2023 03:18:28 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df166fc4715d337f554c5b6904774af766db5e850d3500e12eeafae147f25b5`  
		Last Modified: Fri, 28 Jul 2023 03:29:39 GMT  
		Size: 144.8 MB (144829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520913abe5915f92943fc5c04aaca324e8ede1473e9e297808bc0e5053bc6ba`  
		Last Modified: Fri, 28 Jul 2023 03:30:08 GMT  
		Size: 13.9 MB (13861372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ca29f1435ece222c0bb79f6d28ffbe7da37f9cabb417159d38b17e18a9d754`  
		Last Modified: Fri, 28 Jul 2023 03:30:08 GMT  
		Size: 4.4 MB (4399265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.10.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:10c1a7712e08a95193182f360c2bff0cf83e9e20b33720ef4c05b687d348ba63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.5 MB (213518914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e459901ab3cb0571e10b010fc9f5caf2cccaf9ad40385706777ce45a50f57a3`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:29:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:20:57 GMT
COPY dir:ddfd64e7bd36f630cd100cf454a9685f9fd0f9483467dbf7a4c9a71ab0af7089 in /opt/java/openjdk 
# Tue, 08 Aug 2023 20:21:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:22:50 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 08 Aug 2023 20:22:50 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 08 Aug 2023 20:22:50 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 20:23:04 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 08 Aug 2023 20:23:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 08 Aug 2023 20:23:04 GMT
ENV LEIN_ROOT=1
# Tue, 08 Aug 2023 20:23:06 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 08 Aug 2023 20:23:06 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407c6d757b759af4edf90fb98cce4e2d9dcbe1dbefa7c50cb1db816f3fc06be8`  
		Last Modified: Tue, 08 Aug 2023 20:32:30 GMT  
		Size: 141.6 MB (141565363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191844530d9733e4dc05c6a58929d9339bf4a7310be6ecb0fa3675df0313b571`  
		Last Modified: Tue, 08 Aug 2023 20:33:29 GMT  
		Size: 13.8 MB (13849486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0686f863034585d0ef1db6f21c6f1fbe9a2e1af2adb752a68dee718e09c308`  
		Last Modified: Tue, 08 Aug 2023 20:33:28 GMT  
		Size: 4.4 MB (4399275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
