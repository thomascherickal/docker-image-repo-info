## `clojure:temurin-17-lein-bullseye`

```console
$ docker pull clojure@sha256:b4e6f88a5fb4f1d34e4c0665bcb28c8a98134e186de33274114920121c4f9b70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-lein-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:43c9035f1619a4dd8a5be45a2fe382e9a981e5031c1d59718f866090ce13fd0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265751573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eef35a15f54a40f5932e2284d62637a8185c36cafca9066e100acf722cf52ec`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:11 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:16:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:17:14 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 08:17:14 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:17:15 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:17:29 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 08:17:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:17:30 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 08:17:32 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 08:17:32 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:17:32 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:17:32 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc37eb9b838f833285a35e624da1bfed81e650837c6751e8a6812e51ef22b6ba`  
		Last Modified: Wed, 12 Apr 2023 08:24:36 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7638bac5f42074ab84029ec00a71e757be2b3cb8747bc3dc398c060683172faf`  
		Last Modified: Wed, 12 Apr 2023 08:25:11 GMT  
		Size: 13.9 MB (13860898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287772f564f6ffa8bddd9d5d50416406d0eff16a8c0f4964831ebf6aaa64a475`  
		Last Modified: Wed, 12 Apr 2023 08:25:10 GMT  
		Size: 4.4 MB (4399277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5280a9c90e2639a92319f10f00711e812e61137b21d64cd0a57deb374c2068`  
		Last Modified: Wed, 12 Apr 2023 08:25:10 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-lein-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:56e6b5fa76a5ad0855beaf668f030fc46615dc778ed16f1a23a4071bc18cdffc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263214599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:515f4ac33449f49ed2dffec81342c7b8774d4218454546426735ec970796c3c8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:04 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:23:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:24:10 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 01:24:10 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:24:11 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:24:26 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 01:24:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:24:26 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 01:24:28 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 01:24:28 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:24:28 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:24:28 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6911e57ac771aafcbe41270c1285de884dc5ce0d79a1b3069ec89c3a65e4a6c2`  
		Last Modified: Wed, 12 Apr 2023 01:30:58 GMT  
		Size: 191.3 MB (191260417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e952a0e9e828d9133da5744babc708e5415c7172457fbbd47bcf602a6d73072b`  
		Last Modified: Wed, 12 Apr 2023 01:31:29 GMT  
		Size: 13.8 MB (13848977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9c0590a5e14ae5f3345cbc2b3aa8e425ed3878d7a1910abc64e8dfd4bd85a0`  
		Last Modified: Wed, 12 Apr 2023 01:31:28 GMT  
		Size: 4.4 MB (4399276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e905619cc1ae210071fab26d8eef4d9f11d9d8374cfa6bd8938db45eccde1ef6`  
		Last Modified: Wed, 12 Apr 2023 01:31:27 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
