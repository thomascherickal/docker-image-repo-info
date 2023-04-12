## `clojure:temurin-20-lein-bullseye-slim`

```console
$ docker pull clojure@sha256:e10701172ae857095db73fff056c7cacc04abc8137850d1411ca326e76154822
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-lein-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:c7caeb3567684b7b65deccd2545fbeb1041433bd9240a38d5fb5e9a316e4a675
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251194733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d4266dfd0b30cea343f65f84c44d4a0a7bc9c16bb8b2bac1be5de93424062a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:19:17 GMT
COPY dir:0f9b663d61413099f20817ab55258941c09987290b8ce360d0fb2fab00ddddda in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:19:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:19:19 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 08:19:19 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:19:19 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:19:33 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 08:19:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:19:33 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 08:19:36 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 08:19:36 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:19:36 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:19:36 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b32b49a5ad9ee1b838c8a414680cfb573b6bf63d15cefb9f67402b317700b6`  
		Last Modified: Wed, 12 Apr 2023 08:26:44 GMT  
		Size: 202.8 MB (202800600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9768d1cbee915a6744a46ba57ac06a9562f07072f52a1ae9b125a508fab7d65`  
		Last Modified: Wed, 12 Apr 2023 08:26:31 GMT  
		Size: 12.6 MB (12576302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decbcce718c2bb92774cd4437a2ac9d6fdcb25a4c4b0572d8cf4563b18f1183c`  
		Last Modified: Wed, 12 Apr 2023 08:26:30 GMT  
		Size: 4.4 MB (4399204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcdd7ea80acbe33f6e3f67e4c99621fb6bd1cc43770fdfa0a2d305dade96e70`  
		Last Modified: Wed, 12 Apr 2023 08:26:30 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-lein-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a13db0984a13ea678c63d63b7f52fe592094b97e86461489051c3e99ce69511a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248187230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b469ec762203a6c33d3e013d8ea8a2f0a91698441518a46e610bdb9d9481942`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:25:57 GMT
COPY dir:66b65f1974fed4b5bc3675e6b378c93a3ba9feeabfec7eeabd6d1d0b07fd5fa4 in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:26:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:26:01 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 01:26:02 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:26:02 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:26:17 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 01:26:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:26:18 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 01:26:20 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 01:26:20 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:26:20 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:26:20 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ac14b41f3aaaeba0605fc04f599b4365bfd232c1b3f11a8c1c5c7c4cceaa9b`  
		Last Modified: Wed, 12 Apr 2023 01:32:54 GMT  
		Size: 201.2 MB (201160129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a19f96a1b0ec4b76d42a47f92f9ee41dce2353ba935f7ffc9352f2d38b178b7`  
		Last Modified: Wed, 12 Apr 2023 01:32:43 GMT  
		Size: 12.6 MB (12563648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5856acee58889fd65ee03a2b5b9d263c4ee36981211e2e38e4c00f08555ef0`  
		Last Modified: Wed, 12 Apr 2023 01:32:43 GMT  
		Size: 4.4 MB (4399230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3165832ea3c52d13e5862fbe1160d8b26454f2b4337d0f8fea671181890c3c`  
		Last Modified: Wed, 12 Apr 2023 01:32:42 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
