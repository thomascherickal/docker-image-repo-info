## `clojure:temurin-20-lein-bullseye`

```console
$ docker pull clojure@sha256:126448b5f4ff7bfe3306f186113e7f651deb19eff63959591e35a7de1108f934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-lein-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:8dba783d1671a84df98d39a5159c3743d1e9580c0b810e8db8f8c82bb0f6f2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **276.1 MB (276130039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50109a68cbafe86222b9f6156d10dbc0ae49d63e4dff28475e133086c69df0e2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:52:38 GMT
COPY dir:02736280d197ac4d1b6ebf68d948efb46e7eeffd579505356f8c94946dbcce6f in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:52:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:52:40 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 13 Jun 2023 03:52:40 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:52:40 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:52:54 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 13 Jun 2023 03:52:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:52:55 GMT
ENV LEIN_ROOT=1
# Tue, 13 Jun 2023 03:52:57 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 13 Jun 2023 03:52:57 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:52:57 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:52:58 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff552612282fa24c92a5dfa87c11041f0b4f4d7cd27c3ce8fb2a67f243f9330`  
		Last Modified: Tue, 13 Jun 2023 04:00:38 GMT  
		Size: 202.8 MB (202814025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4837f104a2b9d2ca53b0b886eb0ae75717788a986638956f220b272f9a20ea`  
		Last Modified: Tue, 13 Jun 2023 04:00:25 GMT  
		Size: 13.9 MB (13861183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76253db8ae998bedc118ede224d4f2a45ad1bb0722ff452ebc11a239d901fbb9`  
		Last Modified: Tue, 13 Jun 2023 04:00:24 GMT  
		Size: 4.4 MB (4399271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5760bf11cc3df476f58309f365b9711f3ad5076c74fd51c66336a7504f4120f4`  
		Last Modified: Tue, 13 Jun 2023 04:00:24 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-lein-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:13d10782edceabfacfbe5f4d105e6d2d19c8f818ab37feeef1b86c73947c0b9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.1 MB (273111208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:916966131c9e6785fbe73f902263c4db74e5ac6bbca243823dbc7a2eed8b05d9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:57:52 GMT
COPY dir:f555428af67a610819205eec573e23f479077e0999818ee9dc0f3375599d21db in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:57:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:57:57 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 13 Jun 2023 04:57:57 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 04:57:57 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:58:10 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 13 Jun 2023 04:58:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 04:58:11 GMT
ENV LEIN_ROOT=1
# Tue, 13 Jun 2023 04:58:13 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 13 Jun 2023 04:58:13 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 04:58:13 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 04:58:13 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7fbc4a56457275b512e08117bbea540a06635c8ef73e73b83254270abe2921`  
		Last Modified: Tue, 13 Jun 2023 05:04:44 GMT  
		Size: 201.2 MB (201158012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b14a6768677a8ecb65b1eb3161624ffa1665099c83df372793c5368a0a378a3`  
		Last Modified: Tue, 13 Jun 2023 05:04:33 GMT  
		Size: 13.8 MB (13849391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485c2d4175b2384179f5cbfb3778e4aa24b69819409d4fde12a959a9ff460579`  
		Last Modified: Tue, 13 Jun 2023 05:04:32 GMT  
		Size: 4.4 MB (4399272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab9efa2ab384236e6d0dfd68eef8bf7b436bc8ad3fbe7a2ffd569087fc0d253`  
		Last Modified: Tue, 13 Jun 2023 05:04:32 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
