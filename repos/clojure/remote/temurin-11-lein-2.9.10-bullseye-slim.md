## `clojure:temurin-11-lein-2.9.10-bullseye-slim`

```console
$ docker pull clojure@sha256:c7a105111e16c556fd9cd52b99953701bbd5af5893483e005939f5e771ed836c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.9.10-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:c61003154defd155d8c748ba600f06c2cb0497000ee721aa91cadadc57f203de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246926748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb8646a4db34535a26d169c052670ba69e25b378ccf4ce509d8dc2556fc70d0`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:36:56 GMT
COPY dir:e3c63d67b32fccda756dd62000a0cf47da966d18fe6f1f25cd1f37b60881f0ec in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:36:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:37:59 GMT
ENV LEIN_VERSION=2.9.10
# Tue, 25 Oct 2022 02:37:59 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:37:59 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:38:15 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 25 Oct 2022 02:38:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:38:15 GMT
ENV LEIN_ROOT=1
# Tue, 25 Oct 2022 02:38:18 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 25 Oct 2022 02:38:19 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baa79e738b7c5239823844cc2dde0b88b3b0c50dc1863902d1c9a329b737a80`  
		Last Modified: Tue, 25 Oct 2022 02:50:28 GMT  
		Size: 198.1 MB (198124970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f5c0566e632ee63d92ebb923e6196af9b2a8303de192b1251e96085d1af720`  
		Last Modified: Tue, 25 Oct 2022 02:50:55 GMT  
		Size: 13.0 MB (12983040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913d33250a1ecb7b74df4a61255e4d157675c73f643ee6a8fb0d8d80a050488a`  
		Last Modified: Tue, 25 Oct 2022 02:50:54 GMT  
		Size: 4.4 MB (4398700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.9.10-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8b5f7b62ee5ebc3bb0fb2cefc8f5f521c339d5aacdcfb87325898d889ba108df
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242299882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de4deba2878150751f847e82d933c91f4d4eedbcd7018ca72f4a842d488a3503`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:38:30 GMT
COPY dir:0c9c8c2b9cd43799d246d5824c591352650ad79f5d15544287f00c2deb1e4608 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:38:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:40:56 GMT
ENV LEIN_VERSION=2.9.10
# Wed, 26 Oct 2022 15:40:56 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:40:56 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:41:30 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 26 Oct 2022 15:41:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:41:30 GMT
ENV LEIN_ROOT=1
# Wed, 26 Oct 2022 15:41:32 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 26 Oct 2022 15:41:32 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3d7b35da3e357173d5404cc59df1a4394d6031ee4598b02de7918d2110bae`  
		Last Modified: Wed, 26 Oct 2022 15:58:03 GMT  
		Size: 194.9 MB (194866982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c44e41527d516e9036d2f5ed4c9f4e14e45c9b45acafc86b9ca980b674d5a9`  
		Last Modified: Wed, 26 Oct 2022 15:58:56 GMT  
		Size: 13.0 MB (12970299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7790c4a60adc7dcf8539f8772b2ae24c1f3f64b9798a29188a6b70a57a91411`  
		Last Modified: Wed, 26 Oct 2022 15:58:56 GMT  
		Size: 4.4 MB (4398691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
