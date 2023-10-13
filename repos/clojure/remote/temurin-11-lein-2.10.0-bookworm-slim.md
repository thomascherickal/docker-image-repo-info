## `clojure:temurin-11-lein-2.10.0-bookworm-slim`

```console
$ docker pull clojure@sha256:b133f6c35c2cce1a2cd2845e02be16268712161ac7388d9010cb6cbd2c6a9eaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.10.0-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a742a76d6fcd04479f16b529d5dcc25e4e4a33d7b70432aa2dff2d0ef707fa60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.4 MB (193376565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9182bb1bb4435798a8606995742e5ba5b5e7f5f9a520667c02659d12834dad`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 01:28:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:44:27 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:44:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:47:43 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 13 Oct 2023 12:47:43 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 12:47:43 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:47:59 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 13 Oct 2023 12:47:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 12:47:59 GMT
ENV LEIN_ROOT=1
# Fri, 13 Oct 2023 12:48:02 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 13 Oct 2023 12:48:02 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58d686df0429bc899b9ad25527714341a548bd057ccf4c6c39ca10ffcf2b6a5`  
		Last Modified: Fri, 13 Oct 2023 13:05:13 GMT  
		Size: 144.8 MB (144826195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290af5222bab6eb33c4a1d0ce374e8f29e18d7485389c3cd83e9841b1656a22c`  
		Last Modified: Fri, 13 Oct 2023 13:06:48 GMT  
		Size: 15.0 MB (15001292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1777245b8144db09650170888ecfcbc6a0847017fc6a153ecc58dffc048d8790`  
		Last Modified: Fri, 13 Oct 2023 13:06:47 GMT  
		Size: 4.4 MB (4399204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.10.0-bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:81f98c1e61426224f39a0dd043cba5e9df7ab1c0b6dda85423eb206d2fdada5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (189973189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b19c3fdb38d6e742af422d86bf7e27e33c26802ee2c4dad09ed4f4786380585`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 00:59:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:12:35 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:12:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:15:10 GMT
ENV LEIN_VERSION=2.10.0
# Fri, 13 Oct 2023 10:15:10 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 13 Oct 2023 10:15:10 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:15:23 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 13 Oct 2023 10:15:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 13 Oct 2023 10:15:23 GMT
ENV LEIN_ROOT=1
# Fri, 13 Oct 2023 10:15:25 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 13 Oct 2023 10:15:25 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7aa7d3902d954c470f86fe2b38acaf6172ca287d14a276c679a36a75e4824`  
		Last Modified: Fri, 13 Oct 2023 10:29:43 GMT  
		Size: 141.6 MB (141570614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7d040354e9a8b8b8f0fbd0f24a7f8951606d135f170525076d55423128f569`  
		Last Modified: Fri, 13 Oct 2023 10:31:10 GMT  
		Size: 14.8 MB (14824029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0e6752829eace2f33ebdbbb5d2df8f03f340fd7461bbbc1157624430963010`  
		Last Modified: Fri, 13 Oct 2023 10:31:09 GMT  
		Size: 4.4 MB (4399262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
