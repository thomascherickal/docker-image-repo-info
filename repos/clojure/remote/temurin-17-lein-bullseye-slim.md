## `clojure:temurin-17-lein-bullseye-slim`

```console
$ docker pull clojure@sha256:6f5dbe3df8d523d519972ecbfe45408a381b4bdd63e875580213cb26f39dd67f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-lein-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:558b63d8f2f8bb59d58daacb60a2c5f5c614d7650533da248f765c17a976f348
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.2 MB (193169477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cedb3cb47f0efd0564168aca3188d1db508fcf80cc0c52c76bb4ed2c7bca221`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 20:48:51 GMT
COPY dir:6777d1f77166c2ecdd8f4eb23f5fd82574aa8a90fd65d6dff981fbb31778a3d1 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:31:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:35:24 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 31 Aug 2023 23:35:24 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 31 Aug 2023 23:35:25 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:36:19 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 31 Aug 2023 23:36:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 31 Aug 2023 23:36:19 GMT
ENV LEIN_ROOT=1
# Thu, 31 Aug 2023 23:36:22 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 31 Aug 2023 23:36:22 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 31 Aug 2023 23:36:22 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 31 Aug 2023 23:36:22 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65006a4851e206ccc53a9bf891b081e6fefbdbe0fcb897d670970fc7f2eff9ea`  
		Last Modified: Thu, 31 Aug 2023 20:51:41 GMT  
		Size: 144.8 MB (144775820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04426b9a8f31cab8bbdeaeb6bbe3c8e4da576cc3971c1f2eed698155b8ecb5f8`  
		Last Modified: Thu, 31 Aug 2023 23:45:46 GMT  
		Size: 12.6 MB (12576339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cded21626e67ab08074f32d000a0628e8ebbe6559280618eecbc442b1790f36`  
		Last Modified: Thu, 31 Aug 2023 23:45:45 GMT  
		Size: 4.4 MB (4399238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139773a1e24212679d22553153ac4654dfd5934e03271060a9df417caa8d8ed2`  
		Last Modified: Thu, 31 Aug 2023 23:45:45 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-lein-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:414cafbfb713e21b7f1f6e08ac60692af68fb6c3f78695046e3491bb6213ec17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190569649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d558d85ce24fe8687f19468bd49a619a34ce1fedb8e8c9488c41d13ea31072e7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:48:00 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:48:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:49:17 GMT
ENV LEIN_VERSION=2.10.0
# Sat, 02 Sep 2023 01:49:17 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 02 Sep 2023 01:49:17 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:49:29 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Sat, 02 Sep 2023 01:49:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Sep 2023 01:49:30 GMT
ENV LEIN_ROOT=1
# Sat, 02 Sep 2023 01:49:32 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Sat, 02 Sep 2023 01:49:32 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Sat, 02 Sep 2023 01:49:32 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 02 Sep 2023 01:49:32 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75390d7bc4a96162e240272aeff28881955f7af498179aa85faecd879748f913`  
		Last Modified: Sat, 02 Sep 2023 01:55:46 GMT  
		Size: 143.5 MB (143543515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488c53ec29a87a609179353dddb9e5bc1e382645c9ada7d9875ec79c166ad20f`  
		Last Modified: Sat, 02 Sep 2023 01:56:28 GMT  
		Size: 12.6 MB (12563717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bbe2c75a4e53ae2cfb3bd46f3bddc96f50e6abd5e3df1d5b65e0ead223bcbe`  
		Last Modified: Sat, 02 Sep 2023 01:56:27 GMT  
		Size: 4.4 MB (4399200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b88bd06344b29319a103a6a7d444fa97a47a5fb23a264399825a1f73d78b135`  
		Last Modified: Sat, 02 Sep 2023 01:56:27 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
