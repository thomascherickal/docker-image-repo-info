## `clojure:temurin-11-lein-2.9.10-bullseye`

```console
$ docker pull clojure@sha256:3666fa9c975981011182d0b0889c5e2f499b2ef9541bd5e15478540dbed32d50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-2.9.10-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:7fc8460a827d41731f1fc5ae4f93f525616fc767f59a2adbe8adba28cead5aeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271837776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67c65c13c468dd43cb24f1af13751f95d8fb828f35d335c4b7850f967e9552fd`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:36:10 GMT
COPY dir:e3c63d67b32fccda756dd62000a0cf47da966d18fe6f1f25cd1f37b60881f0ec in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:36:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:37:35 GMT
ENV LEIN_VERSION=2.9.10
# Tue, 25 Oct 2022 02:37:35 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 25 Oct 2022 02:37:35 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:37:52 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 25 Oct 2022 02:37:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 25 Oct 2022 02:37:52 GMT
ENV LEIN_ROOT=1
# Tue, 25 Oct 2022 02:37:55 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 25 Oct 2022 02:37:55 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e425413bc0ae0b1045fcbc0ad4409b98eeded13a40018b63e55084142fd5a78e`  
		Last Modified: Tue, 25 Oct 2022 02:50:03 GMT  
		Size: 198.1 MB (198124992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e6b4e560e51d884511556ee2b1fd07d2d07b4f65697d65ca214c39d9f8b7ce`  
		Last Modified: Tue, 25 Oct 2022 02:50:45 GMT  
		Size: 14.3 MB (14267783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b787ef46c5df95922565cae2273e1c71ed4a232e90e5630deb4d72dad480771`  
		Last Modified: Tue, 25 Oct 2022 02:50:44 GMT  
		Size: 4.4 MB (4398669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-2.9.10-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8b3e8228c6766d193f8387d39518fa56e1f506d1f9e1a10ab6f6ca816a304241
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.2 MB (267223757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd26973b693cea09b5162f46058144db3e434507d741da10ad56e313c48c4c40`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:37:43 GMT
COPY dir:0c9c8c2b9cd43799d246d5824c591352650ad79f5d15544287f00c2deb1e4608 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:37:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:40:07 GMT
ENV LEIN_VERSION=2.9.10
# Wed, 26 Oct 2022 15:40:07 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:40:07 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:40:40 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 26 Oct 2022 15:40:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:40:41 GMT
ENV LEIN_ROOT=1
# Wed, 26 Oct 2022 15:40:47 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 26 Oct 2022 15:40:47 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a7b51e23fc2e53d8018b07b36bae7b1c261267f2981e18b50be0d7b845881`  
		Last Modified: Wed, 26 Oct 2022 15:57:42 GMT  
		Size: 194.9 MB (194866970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1214d65af4cb3ef5e74e1fa7cfe24dcf9ebcd330584117a1c4481bfbd40f33`  
		Last Modified: Wed, 26 Oct 2022 15:58:46 GMT  
		Size: 14.3 MB (14256105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e93a6565494e81afd81aee8310604d41f4e17be48fe6bf74f6fde174ecd640`  
		Last Modified: Wed, 26 Oct 2022 15:58:46 GMT  
		Size: 4.4 MB (4398716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
