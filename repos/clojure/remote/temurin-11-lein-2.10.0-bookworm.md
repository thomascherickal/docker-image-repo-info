## `clojure:temurin-11-lein-2.10.0-bookworm`

```console
$ docker pull clojure@sha256:8d9769cfcd7d2af0a948117d48fa582789fefb7298a724eac0620a0cc248b13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.10.0-bookworm` - linux; amd64

```console
$ docker pull clojure@sha256:3b44583fad7b1698370ecff4f5377635845f792d87e3c654855699de5446f17a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.8 MB (215840170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5dca3249c468f3bfac4515e7339035ebb638194c25d3843bfabd413052ee09`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 01:26:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:43:54 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:43:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:47:08 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 13 Oct 2023 12:47:08 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 12:47:09 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:47:33 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 13 Oct 2023 12:47:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 12:47:33 GMT
ENV LEIN_ROOT=1
# Fri, 13 Oct 2023 12:47:36 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 13 Oct 2023 12:47:36 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312f54f99658b0b7990d26fe3799c0af7d535f77af55acd1d748d19013cad478`  
		Last Modified: Fri, 13 Oct 2023 13:04:52 GMT  
		Size: 144.8 MB (144826232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652cd9818bdcb5320c7924bf65cb8b7af09914c808061124ca150a4340953024`  
		Last Modified: Fri, 13 Oct 2023 13:06:38 GMT  
		Size: 17.0 MB (17032420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708cc504c919185c3325edff0290dfd98e0ce907bd5d4903619f389c373869a5`  
		Last Modified: Fri, 13 Oct 2023 13:06:37 GMT  
		Size: 4.4 MB (4399294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.10.0-bookworm` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:acfbdd91f4a9260b5b01610598adccff862cd3c4d79bd442dd7d69dc1f26fd2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212437125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e17703cb93bb88c1a1c08ccbdb1ec2324c424a2006d7a291eba44adb90aa27a`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 00:57:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:12:02 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:12:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:14:50 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 13 Oct 2023 10:14:50 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 10:14:50 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:15:05 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 13 Oct 2023 10:15:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 10:15:05 GMT
ENV LEIN_ROOT=1
# Fri, 13 Oct 2023 10:15:07 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 13 Oct 2023 10:15:08 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf03c8b0dce1ee3013ef26db39e3fea7b1e7c57443f42116088217a57392c8`  
		Last Modified: Fri, 13 Oct 2023 10:29:26 GMT  
		Size: 141.6 MB (141570586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff96905d8c0b8948ba2dbe4b91a30346653b53a7a8c6bd9c38cc46c73ad0c11c`  
		Last Modified: Fri, 13 Oct 2023 10:30:59 GMT  
		Size: 16.9 MB (16854743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a350cbdb8c22139107a32a6ff5dff92527e488d8ac78aaded123cf680ec6f072`  
		Last Modified: Fri, 13 Oct 2023 10:30:58 GMT  
		Size: 4.4 MB (4399218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
