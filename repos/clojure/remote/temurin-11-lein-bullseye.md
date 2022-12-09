## `clojure:temurin-11-lein-bullseye`

```console
$ docker pull clojure@sha256:23649ce0b3386590312f8455a10f316d803010556bef41516ed11762a90184fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:7bae2287473c81c56be3c08597201e3ae03777d8bd58c6491bda2eda88bd4939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271756643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44194068dc53696264d7e5ff85428f99f9aabf309fced697aa0bbd96362ebdef`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:17 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:36:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 22:26:26 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 09 Dec 2022 22:26:30 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 22:26:30 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 22:26:51 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 09 Dec 2022 22:26:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 22:26:52 GMT
ENV LEIN_ROOT=1
# Fri, 09 Dec 2022 22:26:58 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 09 Dec 2022 22:27:00 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561532e76f8a67e2ac0114bf68c5fcb2c640ceb1eff7b0f331d366e73f673768`  
		Last Modified: Fri, 09 Dec 2022 06:53:29 GMT  
		Size: 198.5 MB (198454561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cdd7995287c35471d60424dd3773ef92c65d3de329657cf928324d788f7187`  
		Last Modified: Fri, 09 Dec 2022 22:44:27 GMT  
		Size: 13.9 MB (13861510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d4b22058fa6db7f41bebc8cf5e577733ce80f60555f41523d6a7f01fbaabde`  
		Last Modified: Fri, 09 Dec 2022 22:44:26 GMT  
		Size: 4.4 MB (4399230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:03b639662c16e700d069fb28a554a3ae61df51d9be6411d77653ae8c72ae4d01
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.2 MB (267151756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fface9538ff10db1954d8f3fd92ae27949603d573de794c8006f1cf34eb31f6`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:03:32 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:03:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 21:41:48 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 09 Dec 2022 21:41:48 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 21:41:48 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 21:42:02 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 09 Dec 2022 21:42:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 21:42:02 GMT
ENV LEIN_ROOT=1
# Fri, 09 Dec 2022 21:42:05 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 09 Dec 2022 21:42:05 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1dc93c936f130a0b32765e5801ad37ff3679f9461520ae91ce9b6fa4d65888`  
		Last Modified: Fri, 09 Dec 2022 05:18:13 GMT  
		Size: 195.2 MB (195203416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68b9693a0999494f5a5b4ad64905c0611195bcd43f067e95284a6ae52d03353`  
		Last Modified: Fri, 09 Dec 2022 21:49:45 GMT  
		Size: 13.8 MB (13849913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5bffa34f93b80c7be4f5663edee097b58ef0a439f1e99da21af0875aad3347`  
		Last Modified: Fri, 09 Dec 2022 21:49:44 GMT  
		Size: 4.4 MB (4399281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
