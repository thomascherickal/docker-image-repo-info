## `clojure:temurin-11-lein-bullseye-slim`

```console
$ docker pull clojure@sha256:e14cc9e8395e53d62aee8696ba983dc1151bd0de0516c3208cda385cae71ec27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:7420999e72a98433dd87a52095841e269d59e0f5c5548e81fb29fae6a48fb274
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246862581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950d32507eeea3b53d8b7f5602f2a7cee135e0e6f6acf22ac33151cc2422acd3`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:25:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:26:39 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:26:39 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:26:39 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:26:54 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:26:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:26:54 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:26:57 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:26:57 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd47ba5a657aa609d02aec742af40ac3926ed293ecaeaed859b51a89124f826`  
		Last Modified: Thu, 09 Feb 2023 09:39:10 GMT  
		Size: 12.6 MB (12576127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f97530ba63ffd2f390cfc9fb4ed6e3b8c532bcb672fdfa0e3b5b6a3b8d01703`  
		Last Modified: Thu, 09 Feb 2023 09:39:09 GMT  
		Size: 4.4 MB (4399221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d3e825c9f9c7323a1b10d76c249e81387ebfe9eab0f2d161394a6556d5a00b61
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242265674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f485399c16f0694531c496c842f199d99d6bee5719b347932e8ecba38fcba8ef`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:21:30 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:21:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:22:20 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:22:20 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:22:20 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:22:34 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:22:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:22:34 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:22:36 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:22:36 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf483a916e651ca447c4add0da489b56284ef3ab648f7c4b8b28762f912a1e`  
		Last Modified: Thu, 09 Feb 2023 09:32:44 GMT  
		Size: 195.2 MB (195240411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8095d2fed7e02b1d120ed91486c66aaa92eb6cd515ce39bd233c94043e27b8ba`  
		Last Modified: Thu, 09 Feb 2023 09:33:05 GMT  
		Size: 12.6 MB (12563477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1662c8328f6b01816673aee05606b2eecad9251756ce52bde8373d03d7b41904`  
		Last Modified: Thu, 09 Feb 2023 09:33:04 GMT  
		Size: 4.4 MB (4399277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
