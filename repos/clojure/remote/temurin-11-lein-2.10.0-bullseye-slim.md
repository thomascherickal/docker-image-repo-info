## `clojure:temurin-11-lein-2.10.0-bullseye-slim`

```console
$ docker pull clojure@sha256:2ebad3b977925bef124f1b76c1414c3171dae5a4858f471bd0309271c6abbdef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.10.0-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:d612dab688b962d6b16fb3c59744424f6f35bb71fbbb461dfea74fd9636245fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246869720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f12b5fd78e6c5dbba92a1cf04940321af97843453e9d356e1493d64a5cfae60`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:14:00 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:14:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:15:01 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 08:15:01 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:15:01 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:15:16 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 08:15:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:15:16 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 08:15:19 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 08:15:19 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4791db44f1181a51939f7b21de0fda8d67e0a03b6a5393ac49f8d64eadc56`  
		Last Modified: Wed, 12 Apr 2023 08:23:18 GMT  
		Size: 198.5 MB (198475991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8413a809d4db96e82adf37f9276cfbef58746c36fb3b0454a7b6563f40abf9`  
		Last Modified: Wed, 12 Apr 2023 08:23:37 GMT  
		Size: 12.6 MB (12576284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f186e2446621ca2a4f2b240645ebf60cab4f287c0ed9de145a15594106d990`  
		Last Modified: Wed, 12 Apr 2023 08:23:37 GMT  
		Size: 4.4 MB (4399217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.10.0-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ea4c6899d51d831863db59c2662bf59a2917ff0bfd572ea1409bc17d062f5695
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242269251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54120a173be6ce11e201c297f720102695e424697dbec4a3d679b0ea97b4d73`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:21:10 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:21:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:22:07 GMT
ENV LEIN_VERSION=2.10.0
# Wed, 12 Apr 2023 01:22:07 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:22:07 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:22:21 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 12 Apr 2023 01:22:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:22:21 GMT
ENV LEIN_ROOT=1
# Wed, 12 Apr 2023 01:22:24 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 12 Apr 2023 01:22:24 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2a925b22c34d676c0f7dfea6c5e40dae89a2cd334554f1387adb3b0d65cee9`  
		Last Modified: Wed, 12 Apr 2023 01:29:42 GMT  
		Size: 195.2 MB (195242534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5ff7f9b6b5d01a06c28d6b1d00a9ad324618dc14c82b90efa45e1fb5c52781`  
		Last Modified: Wed, 12 Apr 2023 01:30:01 GMT  
		Size: 12.6 MB (12563671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6700f7d7c3d42978de74a18229c79707fa4f785248007bfbf340de7250d5f2b0`  
		Last Modified: Wed, 12 Apr 2023 01:30:00 GMT  
		Size: 4.4 MB (4399220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
