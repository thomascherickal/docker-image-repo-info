## `clojure:temurin-8-lein-2.10.0-alpine`

```console
$ docker pull clojure@sha256:ae49db1d71702cbc501e78f810669f3fbfe090a1562a6a521fc489ad400607d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-lein-2.10.0-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:53d0cfd5d36c5d010e625a4e5035493ad36f5f2b1da4bf97f4e0aab46f838bf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80437718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e2ce2fa028d2eebebf5432fa3926dca6f68d3292454259225fe23efeda7f1f`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 24 May 2023 23:34:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 24 May 2023 23:34:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 23:34:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 24 May 2023 23:34:29 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 24 May 2023 23:34:29 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 24 May 2023 23:34:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='cfdf8e07c8eeb087b7a2895b90fc0a19986bcff85006f1e2b708e3964909aa8e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 24 May 2023 23:34:36 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 24 May 2023 23:56:24 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 24 May 2023 23:56:24 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 24 May 2023 23:56:24 GMT
WORKDIR /tmp
# Wed, 24 May 2023 23:56:33 GMT
RUN set -eux; apk add --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Wed, 24 May 2023 23:56:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 May 2023 23:56:33 GMT
ENV LEIN_ROOT=1
# Wed, 24 May 2023 23:56:36 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 24 May 2023 23:56:36 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdde4a302e0d0ee2ef6760bf84344d762835ef2d38d2a1a1062c7d038fe2615b`  
		Last Modified: Wed, 24 May 2023 23:37:36 GMT  
		Size: 7.6 MB (7648427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d694a2b7c16a77c50982c0d6c082b7283771de0ec5cc847bd355b7ab684aedc9`  
		Last Modified: Wed, 24 May 2023 23:37:40 GMT  
		Size: 52.5 MB (52539524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d54ff8e92ad62b25089a5c48736e5c228115778e74dc2155361eda232c376ae`  
		Last Modified: Wed, 24 May 2023 23:37:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9f2b1c3c4144aaca39596204f79f29a4cf1609c076f1209d5fbd4accc1219a`  
		Last Modified: Thu, 25 May 2023 00:00:21 GMT  
		Size: 12.5 MB (12452850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a06afd97337b3ecbdc3cf346cf52ce0c68de61ad523e2e75d4b26e4a7d27e6`  
		Last Modified: Thu, 25 May 2023 00:00:21 GMT  
		Size: 4.4 MB (4399267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
