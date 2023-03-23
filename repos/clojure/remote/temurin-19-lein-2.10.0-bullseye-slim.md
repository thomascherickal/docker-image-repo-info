## `clojure:temurin-19-lein-2.10.0-bullseye-slim`

```console
$ docker pull clojure@sha256:4fce8ce2458fca9507ec3ad30229fd35bf95443f9003d6f39d2c19b6878119bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-lein-2.10.0-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:0f531752a9b7de72036fb0cd643689bb961c216c1d3b701472257335b6e2c2b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.5 MB (249500191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e29203f57916e268a025c12551db4370359d4fcfe01506cab951352f02752618`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:25:51 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:25:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:26:48 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 23 Mar 2023 06:26:48 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:26:48 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:27:02 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 23 Mar 2023 06:27:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:27:02 GMT
ENV LEIN_ROOT=1
# Thu, 23 Mar 2023 06:27:04 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 23 Mar 2023 06:27:04 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:27:05 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:27:05 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50160c605f9c02acd78ef392f7194eee61162e99ab69aa71a85d2c04e97ff86`  
		Last Modified: Thu, 23 Mar 2023 06:34:39 GMT  
		Size: 201.1 MB (201112949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c07861819a25b853e233174b4cb875822f704a2a8cda60314347e83e11fd73f`  
		Last Modified: Thu, 23 Mar 2023 06:34:58 GMT  
		Size: 12.6 MB (12576167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32782d78ba6408908f712e5ced1dd113d37acbe27355b1d93b11037e4e848e4`  
		Last Modified: Thu, 23 Mar 2023 06:34:57 GMT  
		Size: 4.4 MB (4399272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f610be284ee1664b2d4bf187fe633c1c76d1c7099c4fa737120c4de8aebebf`  
		Last Modified: Thu, 23 Mar 2023 06:34:57 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-lein-2.10.0-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:78262af3aa4e3f62ce964a55004436d465faed80e8d8761b6e2553501d2d663a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246881062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbfbb2a3cc47c03eba6fbc67106d8a04a0861d00b50c4d3b219931bec479e371`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:59:40 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:59:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:00:33 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 23 Mar 2023 07:00:33 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 07:00:34 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 07:00:47 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 23 Mar 2023 07:00:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 07:00:47 GMT
ENV LEIN_ROOT=1
# Thu, 23 Mar 2023 07:00:49 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 23 Mar 2023 07:00:49 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 07:00:49 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 07:00:49 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274b1a27e7816b7f1e1f1324be385765b25723b5eddb3f339875cd4a1fa13c6e`  
		Last Modified: Thu, 23 Mar 2023 07:07:40 GMT  
		Size: 199.9 MB (199855165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4e062f2bcbc9f9a3d014bab631bb6b5670c6ebbb47d5f75237213564881240`  
		Last Modified: Thu, 23 Mar 2023 07:08:00 GMT  
		Size: 12.6 MB (12563517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334773cd813c70d8175eb38680bdedb34fbfa1b5ded158fc212e9c939dbb4f13`  
		Last Modified: Thu, 23 Mar 2023 07:07:59 GMT  
		Size: 4.4 MB (4399282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ea7be291eae4dfbd35508f44a19ed0435982b1c99cdd51b52921abaca12944`  
		Last Modified: Thu, 23 Mar 2023 07:07:59 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
