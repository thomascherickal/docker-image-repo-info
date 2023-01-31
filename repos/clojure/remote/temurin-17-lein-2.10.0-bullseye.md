## `clojure:temurin-17-lein-2.10.0-bullseye`

```console
$ docker pull clojure@sha256:8033b9b9c660ac96416a9ee2a55e1f3e9b91ef11df2924785cd818c3b5911990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-lein-2.10.0-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:fbbd73d0ab1c06d0d395ee847c1968312f065a3dc83e2b4b71be28a3239170e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.7 MB (265723347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43014c518ee1cdc90e2ef5b86752b5a4d3e59b7cb29bbdc035a1057d4abec538`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:22 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Wed, 25 Jan 2023 00:45:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 00:47:15 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 25 Jan 2023 00:47:15 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 00:47:15 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:47:31 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 25 Jan 2023 00:47:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 00:47:31 GMT
ENV LEIN_ROOT=1
# Wed, 25 Jan 2023 00:47:34 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 25 Jan 2023 00:47:34 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 25 Jan 2023 00:47:34 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 25 Jan 2023 00:47:34 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147288dc8989fb24ee233733fb7ef84c2cf5d7be2f0863fe9ea1e153e52a350f`  
		Last Modified: Wed, 25 Jan 2023 00:57:58 GMT  
		Size: 192.4 MB (192438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3916a89348070dbc7bea6a1f27bf5e541e2c922058f650a7768aff9a164e51`  
		Last Modified: Wed, 25 Jan 2023 00:59:21 GMT  
		Size: 13.9 MB (13860353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e24f02c7292e20fdee96f37cb8d9026dd420fb15a3eb9b9e25c2c3464f0971f`  
		Last Modified: Wed, 25 Jan 2023 00:59:20 GMT  
		Size: 4.4 MB (4399224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8880fc956ab8a7a57a7d388e553cb9f1a6676e2341919b11f40a41df757357f2`  
		Last Modified: Wed, 25 Jan 2023 00:59:20 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-lein-2.10.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:459d633603150a6a38e041daf40b444f6e0e2e03753aac61803f792f9f6613b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263190326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:432c6e1d276014fab949cf8c00097ff35705d371ef108e3124f864f48b44df4a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:01 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 20:54:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:55:32 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 31 Jan 2023 20:55:32 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 31 Jan 2023 20:55:32 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:55:45 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 31 Jan 2023 20:55:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 31 Jan 2023 20:55:45 GMT
ENV LEIN_ROOT=1
# Tue, 31 Jan 2023 20:55:48 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 31 Jan 2023 20:55:48 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Tue, 31 Jan 2023 20:55:48 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 31 Jan 2023 20:55:48 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f61d91708311a5923680a9fa5ce56fc7a173443a91b20c1941a3baab459e19`  
		Last Modified: Tue, 31 Jan 2023 21:07:15 GMT  
		Size: 191.3 MB (191260441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbefec41f4a294d15b8dba56725e69e4db55dc5d429b593bbb0a211acb483b9`  
		Last Modified: Tue, 31 Jan 2023 21:08:23 GMT  
		Size: 13.8 MB (13848406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7ddd7f894d3bc5c9c702f1f14dded642362a0425e5e5a5d4d5a058e2712128`  
		Last Modified: Tue, 31 Jan 2023 21:08:23 GMT  
		Size: 4.4 MB (4399220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2f84b8de3a07110ca4b8b00f56e6cab01589d47825ec44825f4bf3629ba56`  
		Last Modified: Tue, 31 Jan 2023 21:08:22 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
