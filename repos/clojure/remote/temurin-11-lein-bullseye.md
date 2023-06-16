## `clojure:temurin-11-lein-bullseye`

```console
$ docker pull clojure@sha256:c64f90dfc966662a6388d3de24ccf41a9d14cfdfe36ebf813099699edcb9965b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:fe01fdaef4ff2dad7cb7af636c07bcbf2ff2ea54be7dd1c9ef1c8b23dc6ab7b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.9 MB (271865309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:229b66f7024ed08a8c57fbe3d4dcd0826055d5ee40645871a403f867cf94fdbb`
-	Default Command: `["lein","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:46:56 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:46:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:48:08 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 13 Jun 2023 03:48:08 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:48:08 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:48:22 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 13 Jun 2023 03:48:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:48:22 GMT
ENV LEIN_ROOT=1
# Tue, 13 Jun 2023 03:48:25 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 13 Jun 2023 03:48:26 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12b8c3d504afe22ba8eb61403c46f5cc24b3d13561e5bdd23c0feed04b5a618`  
		Last Modified: Tue, 13 Jun 2023 03:57:02 GMT  
		Size: 198.5 MB (198549757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08831c28b28078428e6670babdec6dde05b8d5712b498c440c9ae6f4697f0219`  
		Last Modified: Tue, 13 Jun 2023 03:57:35 GMT  
		Size: 13.9 MB (13861124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ec57736d1dfc6b2e7b11c6bb60988a4274903293f0d97c15e1cf99627ae286`  
		Last Modified: Tue, 13 Jun 2023 03:57:34 GMT  
		Size: 4.4 MB (4399266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:69bdc0164b16d346662902e875dce9c770569c6ec36618ac9a773755f09330ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.3 MB (267276982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e2ecfe3e26dbd6a8114301cda8ab36d2b8bf0650254415941750cd025f3d94`
-	Default Command: `["lein","repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 04:41:42 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Fri, 16 Jun 2023 04:41:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:43:44 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 16 Jun 2023 04:43:44 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 16 Jun 2023 04:43:44 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:44:06 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 16 Jun 2023 04:44:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 16 Jun 2023 04:44:06 GMT
ENV LEIN_ROOT=1
# Fri, 16 Jun 2023 04:44:08 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 16 Jun 2023 04:44:08 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b429dc913a313200e2709dc18ae8c848cf538439e00d089ddee5b4541385cd44`  
		Last Modified: Fri, 16 Jun 2023 04:54:03 GMT  
		Size: 195.3 MB (195324188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb74dd89a91f0acc8473dc0c48d3ecd1ff6ef814dc4ed5650b08ef13cbeae96`  
		Last Modified: Fri, 16 Jun 2023 04:55:02 GMT  
		Size: 13.8 MB (13849386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5170625623a64f0f91a9a588666821396c5597ec7830dcf4b758aff9f2a5c02`  
		Last Modified: Fri, 16 Jun 2023 04:55:02 GMT  
		Size: 4.4 MB (4399272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
