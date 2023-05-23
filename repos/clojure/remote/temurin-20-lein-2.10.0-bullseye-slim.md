## `clojure:temurin-20-lein-2.10.0-bullseye-slim`

```console
$ docker pull clojure@sha256:606721a82f91c65f29cd44c6185276052e1583b84928d178f626ec0783dd9ed3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-lein-2.10.0-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:6a9931b9529a5ad8ff0aa3ca0f767b679e513d7891a2664427b36526689b45e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251193381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a050710191572991c84c2132a4824ae6fae495f9c0d4c6c949e36eb00794602`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:32:51 GMT
COPY dir:02736280d197ac4d1b6ebf68d948efb46e7eeffd579505356f8c94946dbcce6f in /opt/java/openjdk 
# Wed, 03 May 2023 20:32:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 20:32:53 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 03 May 2023 20:32:53 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 03 May 2023 20:32:53 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:33:40 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 19 May 2023 20:33:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 19 May 2023 20:33:41 GMT
ENV LEIN_ROOT=1
# Fri, 19 May 2023 20:33:44 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 19 May 2023 20:33:44 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Fri, 19 May 2023 20:33:44 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 19 May 2023 20:33:44 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02720e2873c980e5fcc584b01ace091e5d4d05cd22a426e5b195f3d93f338875`  
		Last Modified: Wed, 03 May 2023 20:40:25 GMT  
		Size: 202.8 MB (202813964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ea440bd85d4e53c9048031d4100773038fb034788604c290ffad67ac97c1d8`  
		Last Modified: Fri, 19 May 2023 20:44:06 GMT  
		Size: 12.6 MB (12576279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0917087b42af3762215315094f7d5b72acf7fc7fd3c4728074a2fecadf9986cf`  
		Last Modified: Fri, 19 May 2023 20:44:06 GMT  
		Size: 4.4 MB (4399222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e15c78f57e97e0d5eedfea3e8f2ab8d4156d6583eb50c7431419cb56a1db51f`  
		Last Modified: Fri, 19 May 2023 20:44:05 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-lein-2.10.0-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2297ff61dcbf795c26ac6a187177eea89cf8f332327ae45768b99a9160620b9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248174098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:216a510c4fc418ef44cb8f1717aa22d65d4683d5024cd541f3dbeffec02e898d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:32:09 GMT
COPY dir:f555428af67a610819205eec573e23f479077e0999818ee9dc0f3375599d21db in /opt/java/openjdk 
# Tue, 23 May 2023 01:32:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:32:13 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 23 May 2023 01:32:13 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 23 May 2023 01:32:13 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:32:27 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 23 May 2023 01:32:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 23 May 2023 01:32:27 GMT
ENV LEIN_ROOT=1
# Tue, 23 May 2023 01:32:29 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 23 May 2023 01:32:29 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Tue, 23 May 2023 01:32:29 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 23 May 2023 01:32:29 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a408f7150c3feef58c3abe2b486974c10a4d64c30a1c85440e6c6590693f6963`  
		Last Modified: Tue, 23 May 2023 01:39:01 GMT  
		Size: 201.2 MB (201157995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7753de645c4f266ddbd8d028a12e80a5dbc57dccdc6ec2a68c6b4043462b0cac`  
		Last Modified: Tue, 23 May 2023 01:38:50 GMT  
		Size: 12.6 MB (12563671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c60904c58e7b3490f066e0115d2332b967ad81846b83de35a678b2ca94ed3b`  
		Last Modified: Tue, 23 May 2023 01:38:50 GMT  
		Size: 4.4 MB (4399285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf20dc8d5ac45e8be6b1ed6e1af8646d37b43181adb46700880dabc7e3da80c`  
		Last Modified: Tue, 23 May 2023 01:38:49 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
