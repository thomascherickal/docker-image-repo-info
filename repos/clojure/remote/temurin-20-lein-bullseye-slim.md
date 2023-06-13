## `clojure:temurin-20-lein-bullseye-slim`

```console
$ docker pull clojure@sha256:6cce6bfb5110843c7994def242fd7be0e29c4040a73f66bfe5f011b754b2f66c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-lein-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b02145621c6ac0d0e1d928b0f61c16bdcb40865888d4b1b52d64e0811696575b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251207259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e091b7cfb3029b930eb55346ed3f070261c9afafda818f730fc6a41c2f61c7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:53:06 GMT
COPY dir:02736280d197ac4d1b6ebf68d948efb46e7eeffd579505356f8c94946dbcce6f in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:53:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:53:08 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 13 Jun 2023 03:53:08 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 03:53:08 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:53:22 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 13 Jun 2023 03:53:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 03:53:22 GMT
ENV LEIN_ROOT=1
# Tue, 13 Jun 2023 03:53:25 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 13 Jun 2023 03:53:25 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:53:25 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:53:25 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ed12ffb6e1c454a1384074f474bd403cef6b65d6e8b73d5640a4874312de`  
		Last Modified: Tue, 13 Jun 2023 04:01:02 GMT  
		Size: 202.8 MB (202813962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28399e0a595ec3e14facff16002d61ca46e073d5b62a7da7c6fdaff5bc8f47e3`  
		Last Modified: Tue, 13 Jun 2023 04:00:49 GMT  
		Size: 12.6 MB (12576259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43db3c2d620c2805d465c047c7536f6ad7de360c3ab3a36382e7ccd21080bb73`  
		Last Modified: Tue, 13 Jun 2023 04:00:48 GMT  
		Size: 4.4 MB (4399230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6282fb2482707ed3f74c79cdd472c18e3a2340ba43c70a41f24711e37709d29`  
		Last Modified: Tue, 13 Jun 2023 04:00:48 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-lein-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:36308799692387d4a7f1fdc5d949be56a9a0a48b553e5bed82a869be3b991b8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248184153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d85ffaee4ecbe878729bbcb2b3c95ecca32fa640f3e6c382443b3a65a30e8f3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:58:18 GMT
COPY dir:f555428af67a610819205eec573e23f479077e0999818ee9dc0f3375599d21db in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:58:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:58:23 GMT
ENV LEIN_VERSION=2.10.0
# Tue, 13 Jun 2023 04:58:23 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 13 Jun 2023 04:58:23 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:58:36 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 13 Jun 2023 04:58:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 13 Jun 2023 04:58:36 GMT
ENV LEIN_ROOT=1
# Tue, 13 Jun 2023 04:58:39 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 13 Jun 2023 04:58:39 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 04:58:39 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 04:58:39 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec330e2c6a276c3efe415a805c40d111b657a3b03708c5cd4d818fdca4560f53`  
		Last Modified: Tue, 13 Jun 2023 05:05:04 GMT  
		Size: 201.2 MB (201157962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714926e306705250b65a16fdc9c3dd7d31c0d4d452023448fed3c763773b45ca`  
		Last Modified: Tue, 13 Jun 2023 05:04:53 GMT  
		Size: 12.6 MB (12563735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df9b05883f8f132d72242405a47db9514b38355d64c4182282fe2478c6fcb4a`  
		Last Modified: Tue, 13 Jun 2023 05:04:52 GMT  
		Size: 4.4 MB (4399224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755ef6cd65ff6279ccf824df2e2721add1d4f5e1190406bef1678437312945a2`  
		Last Modified: Tue, 13 Jun 2023 05:04:52 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
