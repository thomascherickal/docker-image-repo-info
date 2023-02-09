## `clojure:temurin-8-lein-bullseye-slim`

```console
$ docker pull clojure@sha256:5b2000f78cd8d49bd15ee8bbb4f985a4f3589f43b60a6e4946f08dc30ab18b89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-lein-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:84870a5f0ef0f689ae1dc5db15ea2651f70edd9b12ad9a9a16091dfb79474716
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (103022784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8835989fb94c172c0a9f8f94023a57fd236950836090dc15e1440e653a3dd680`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:22:39 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:22:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:23:36 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:23:36 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:23:36 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:23:51 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:23:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:23:51 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:23:54 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:23:54 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff09d33db7932dfdb13e1ebfdd9d02620a26713de0236d8aef1f5d2e115b133`  
		Last Modified: Thu, 09 Feb 2023 09:36:59 GMT  
		Size: 54.6 MB (54635563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b68bf118b6148aadccaa17245d405dcafb969725e42e278aa733dc271a7b7b`  
		Last Modified: Thu, 09 Feb 2023 09:37:20 GMT  
		Size: 12.6 MB (12576134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518af77c0b77a3960e08c9c9a69974e9ea0228a4bf60d291fbe64bdb133c65c3`  
		Last Modified: Thu, 09 Feb 2023 09:37:19 GMT  
		Size: 4.4 MB (4399277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-lein-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5d5b1b14c75357abc2a06e3fd19b37185351873c48b661f30cdbc2cf28aadaef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100753122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:544abdb276e0bca67c5aae229b68bd2c620eb1adfc7517aa6ba885f62ab3731e`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:18:59 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:19:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:19:51 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:19:51 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:19:51 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:20:04 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:20:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:20:04 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:20:06 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:20:06 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd68f0bab68b42136c4251287a12f055f74853a5f1d694a98637f9f09e4ed94`  
		Last Modified: Thu, 09 Feb 2023 09:31:02 GMT  
		Size: 53.7 MB (53727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae8a0432a768143935fe112df5492d9cf89a30b90284fb1261bce1b1c08f71f`  
		Last Modified: Thu, 09 Feb 2023 09:31:23 GMT  
		Size: 12.6 MB (12563469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687fe3969e8439752c78b03b3fc749b0d178717a758947e8ab4db7f52efe050c`  
		Last Modified: Thu, 09 Feb 2023 09:31:22 GMT  
		Size: 4.4 MB (4399225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
