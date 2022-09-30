## `clojure:temurin-19-lein-2.9.10-bullseye-slim`

```console
$ docker pull clojure@sha256:15ce564788901b983e6a94504705e39b3f68c912bedb97afafee4d8781baafe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-lein-2.9.10-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:e8f9180fa39231c5ee64531aa470957a65713663cd2984798d6af88ef0d86199
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249628393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be5b4c482222674c4ffdf2230eeca2ce4439fdb1ef41c07d592d891e341a082`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:30:53 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:30:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:31:56 GMT
ENV LEIN_VERSION=2.9.10
# Fri, 30 Sep 2022 22:31:56 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:31:56 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:32:12 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 30 Sep 2022 22:32:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:32:12 GMT
ENV LEIN_ROOT=1
# Fri, 30 Sep 2022 22:32:15 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 30 Sep 2022 22:32:15 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:32:15 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:32:15 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bbd00616de1dc5ce1c327c999f5b62b49d54d9d1aecb11cb2cc05bf8fd679d`  
		Last Modified: Fri, 30 Sep 2022 22:41:57 GMT  
		Size: 200.8 MB (200843777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccc13ac9b29dfa4f417151091390589d26497d251250fb2fc1d535fba058236`  
		Last Modified: Fri, 30 Sep 2022 22:42:21 GMT  
		Size: 13.0 MB (12981426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b87f8d847808b8467d22fdb556513b36257ae6c5700c7c1c0c611b5bcb29a65`  
		Last Modified: Fri, 30 Sep 2022 22:42:20 GMT  
		Size: 4.4 MB (4398668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678ffcf223edbc555a31c30012cf68c9a267915842e26e4e16220ac1b9c7ca5b`  
		Last Modified: Fri, 30 Sep 2022 22:42:20 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-lein-2.9.10-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:67c25ff81f5834c5bbe8401f4dce07d42ee16a4deb28fb5590162feb7fab020f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (247004713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265ca601c4fdac029170099a2dd57c09bedc519865db289146c4e89b171c87a0`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:52:28 GMT
COPY dir:58f6c37df253d3555e493197f96e3f21593e31d3faf1967e0a7b9d8f0ae9e30c in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:52:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:53:57 GMT
ENV LEIN_VERSION=2.9.10
# Fri, 30 Sep 2022 22:53:58 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:53:59 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:54:23 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 30 Sep 2022 22:54:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:54:24 GMT
ENV LEIN_ROOT=1
# Fri, 30 Sep 2022 22:54:27 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 30 Sep 2022 22:54:29 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:54:29 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:54:30 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e88c33693f932839a1b6d9254e2e1ad8799153952e412da2891fa1679ec8b`  
		Last Modified: Fri, 30 Sep 2022 23:07:34 GMT  
		Size: 199.6 MB (199582874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b26c48092d12a72e1a98c5450adcc5261287b0a03a38772a4ae1670cd4bf13`  
		Last Modified: Fri, 30 Sep 2022 23:08:00 GMT  
		Size: 13.0 MB (12968589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb75148745388073a3e78e509347693985f4794c2548f4dbb0f86c473715d0d6`  
		Last Modified: Fri, 30 Sep 2022 23:07:59 GMT  
		Size: 4.4 MB (4398610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8e4619d6ecad2eea206c536d8075f56cd974a3bb8f39b67946583e31bd56f0`  
		Last Modified: Fri, 30 Sep 2022 23:07:59 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
