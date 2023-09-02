## `clojure:temurin-11-lein-2.10.0-bullseye`

```console
$ docker pull clojure@sha256:8a16137bdd69fa978f1781233b33494586ea42fc18310969c8cfbd4909c911cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.10.0-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:8c6210c621fc8ca1f74b8660e05da21487e74f03021e1b165634d90e0100b29d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.1 MB (218143364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993216d9cb57f98019a5243561c6a737cbf2819a8669df2f1975163f0ffca2ec`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 23:22:26 GMT
COPY dir:9c2351d5d5cdf669213a7cfcfa52bd6bd8e9fc36b0a8e93328276d7280e1bab3 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:22:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:25:14 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 31 Aug 2023 23:25:14 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 31 Aug 2023 23:25:14 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:25:59 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 31 Aug 2023 23:25:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 31 Aug 2023 23:25:59 GMT
ENV LEIN_ROOT=1
# Thu, 31 Aug 2023 23:26:02 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 31 Aug 2023 23:26:02 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab352bd56ec5464a5d56238b020eb3ec17516ac2525535fdf339dacbad129b6`  
		Last Modified: Thu, 31 Aug 2023 23:41:03 GMT  
		Size: 144.8 MB (144826073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0406af34926b4167e48281e06b66c0f22b1a00eb692709a15051ff0b6b0275`  
		Last Modified: Thu, 31 Aug 2023 23:42:01 GMT  
		Size: 13.9 MB (13861377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fce7bb621e34ce6e055b1a24307da4ee6b5051cb8f751fe1dff8f926e29348`  
		Last Modified: Thu, 31 Aug 2023 23:42:01 GMT  
		Size: 4.4 MB (4399293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.10.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:75288888bdb55e9b3d0da6729cf26e513e2522c3dc222934187965ef3fdd3979
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.5 MB (213523869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a31b4aa9589bca72ebc30f4b82b3c9558a2739c2653346fe0029ad42c15581e8`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:43:53 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:43:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:45:27 GMT
ENV LEIN_VERSION=2.10.0
# Sat, 02 Sep 2023 01:45:27 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sat, 02 Sep 2023 01:45:27 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:45:43 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Sat, 02 Sep 2023 01:45:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Sep 2023 01:45:43 GMT
ENV LEIN_ROOT=1
# Sat, 02 Sep 2023 01:45:45 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Sat, 02 Sep 2023 01:45:46 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e4e3a8bbfd2bdf093ae59fc74ef766b5e27c2748069f457d192d1719121d34`  
		Last Modified: Sat, 02 Sep 2023 01:53:12 GMT  
		Size: 141.6 MB (141570380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f149432e7c65d28cc7e8d17f40e568bdfe3bac591bd3e0626f8bd4d94314e47`  
		Last Modified: Sat, 02 Sep 2023 01:53:54 GMT  
		Size: 13.8 MB (13849483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dfad6e7d0a947ce0e1ec5d7f4707a8767453f1613900e29658f11ce79a8495`  
		Last Modified: Sat, 02 Sep 2023 01:53:54 GMT  
		Size: 4.4 MB (4399227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
