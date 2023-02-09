## `clojure:temurin-17-lein-bullseye-slim`

```console
$ docker pull clojure@sha256:82dda5d508ee184a3786f47a4f33b22b67549fc8dfcac4bc7dc2e955a3c64b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-lein-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:9cc01f7ec7459165d14245fd377e33a3bfa92d6d22eb9cbf5762df6568c13385
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.8 MB (240825794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fff9f7a97e08ea9a592650dec833786db9272d36fc9451e1d567b135c99025`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:28:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:29:41 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:29:41 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:29:41 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:29:56 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:29:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:29:56 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:29:59 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:29:59 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:29:59 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:29:59 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb60adc0d71bc760d3fbac5059d26bf794695a8db88aeb9010e7abaf0bf7a3`  
		Last Modified: Thu, 09 Feb 2023 09:41:05 GMT  
		Size: 12.6 MB (12576116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ea54cd830b7ac26f820ee8270a31ea9442e227806525d94f888aaa895f8312`  
		Last Modified: Thu, 09 Feb 2023 09:41:04 GMT  
		Size: 4.4 MB (4399277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f234b0813fff21ef088dcfc45124412a7e56f5b32c9583f600bd525643d066b`  
		Last Modified: Thu, 09 Feb 2023 09:41:04 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-lein-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4ef4fef9241081e44e22001bba6467d026cc5f4f9d347e611a0c4f97fad145d8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.3 MB (238286067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8666878d84061f0309ceb6658b53b8eaed8a0e98523df06d225d452037bc4dbe`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:24:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:24:49 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:24:50 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:24:50 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:25:03 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:25:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:25:03 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:25:05 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:25:05 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:25:05 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:25:05 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4ce2deaf6f1fcf00baf863114e0ab378ca55e7027d1dde02d586871596fd71`  
		Last Modified: Thu, 09 Feb 2023 09:34:49 GMT  
		Size: 12.6 MB (12563463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e795256c58a74d0134b8d0de3e7cdd6465f990750ddd12f8f9fada6003dd758`  
		Last Modified: Thu, 09 Feb 2023 09:34:49 GMT  
		Size: 4.4 MB (4399267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33764de912ba464cfdb8daa77a658e25cd628bb99fc063f174324886cdc93960`  
		Last Modified: Thu, 09 Feb 2023 09:34:48 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
