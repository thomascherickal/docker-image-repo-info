## `clojure:temurin-19-lein-bullseye`

```console
$ docker pull clojure@sha256:4e752d8f4ae1949d266fe14d8627ad868e5dc6569ca27168b1f8b284e5f6810c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-lein-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:e9a32648045a436641054833522e0d0228b5a18f20d95547edde111ec108ed9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.4 MB (274420350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56b7764c12eaccfc17efe4631846fbd9e7334ee5f9f5b8a052bcfc0273508c34`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:31:09 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:31:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:32:19 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:32:19 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:32:19 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:32:35 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:32:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:32:35 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:32:38 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:32:38 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:32:38 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:32:38 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441046777b829253c9900fed7834e1437d44d485f4ec90904dc51bc5aac05148`  
		Last Modified: Thu, 09 Feb 2023 09:42:23 GMT  
		Size: 201.1 MB (201112949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db9467006a0a5ce3809e780fd9088c9b464074fc85ed1112e5db831d8af9831`  
		Last Modified: Thu, 09 Feb 2023 09:42:59 GMT  
		Size: 13.9 MB (13860993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ff33871f72660672eb1ec39319a16e09f86314b2e49d155fe0ad000713485`  
		Last Modified: Thu, 09 Feb 2023 09:42:59 GMT  
		Size: 4.4 MB (4399235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f131eecfe8a01f6fba52a74f1cefee58fc239f597acdbbe1a58944911da5c50d`  
		Last Modified: Thu, 09 Feb 2023 09:42:58 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-lein-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:91d77949e97d503f207ec684641082e9e3a40d17a19eb15515c21aa9fb5058b1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271807109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f0a6d0bc989c8325cbd89197c9b53b40fe6391cd5edde0a31e861ddde55b9c6`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:55 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:26:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:26:59 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:26:59 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:26:59 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:27:12 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:27:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:27:12 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:27:14 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:27:14 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:27:15 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:27:15 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04575e4d68cefe99b7db24f9eba8de51503dbe724ee7b0b0862498a73eeefbf3`  
		Last Modified: Thu, 09 Feb 2023 09:36:01 GMT  
		Size: 199.9 MB (199855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0387b7006c5c9401e48a7de87ec52dbd9d73b9b8e4079e78c4ae579f68828e`  
		Last Modified: Thu, 09 Feb 2023 09:36:36 GMT  
		Size: 13.8 MB (13848936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80e7b247e3507e8e75fb6a8bd5b6ee8e335f1e19ee96c68dd0c218bc64c5270`  
		Last Modified: Thu, 09 Feb 2023 09:36:35 GMT  
		Size: 4.4 MB (4399236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3989b6b81bfbfc69211282aaca79125d99ad98d2ce634059f84d48a590d39b`  
		Last Modified: Thu, 09 Feb 2023 09:36:35 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
