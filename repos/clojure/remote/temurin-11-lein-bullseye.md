## `clojure:temurin-11-lein-bullseye`

```console
$ docker pull clojure@sha256:f90096fa85d0822779cd80309c762c06997e7c294860e41a74cf4500c73e2822
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-lein-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:d6d63bb9cb314445250b6b21a35822e4bccc62c8a93368e246613f103b823a14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271782307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17ead50a5c59c54cab06cac7b4540fb41db19ead46a73b800a4119dbc212b3e2`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:04 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:25:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:26:15 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:26:15 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:26:15 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:26:30 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:26:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:26:30 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:26:33 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:26:33 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fa5505d5f9a403b5fa799c74b7639e1188ddc30c0db155b99238ff035c03ed`  
		Last Modified: Thu, 09 Feb 2023 09:38:26 GMT  
		Size: 198.5 MB (198475422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ebaa0790a0e0b5c6035a1cd8fe276c1c71acc834fed6b69c3ced17b77d41d4`  
		Last Modified: Thu, 09 Feb 2023 09:39:01 GMT  
		Size: 13.9 MB (13860913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca9ca33da6567a2f521d774efeec803f84f7f86571eded552418e32a17cca4`  
		Last Modified: Thu, 09 Feb 2023 09:39:00 GMT  
		Size: 4.4 MB (4399201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-lein-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:aefe3bf4cba5810f456ebf5ee8a599807f012f84939e44df76f7a00d6067ca78
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.2 MB (267191859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9758c4953c3938bd33489064429897d7ed018b895da345c5e9a856faf198f30c`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:20:57 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:21:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:22:00 GMT
ENV LEIN_VERSION=2.10.0
# Thu, 09 Feb 2023 09:22:00 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:22:00 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:22:14 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "b1757ce941e4cbf15cbf649b7b4f413365e612da892d22841ec1728391bb66af *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 09 Feb 2023 09:22:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:22:14 GMT
ENV LEIN_ROOT=1
# Thu, 09 Feb 2023 09:22:17 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 09 Feb 2023 09:22:17 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84634f2412fd0db390d1dd82c75871f25a933e1333ec652a66114e5288d4d33f`  
		Last Modified: Thu, 09 Feb 2023 09:32:24 GMT  
		Size: 195.2 MB (195240325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7554e9136958a3b59f8db0cf18d2a5a2238e24b781d6f5b1db76584670d5528`  
		Last Modified: Thu, 09 Feb 2023 09:32:56 GMT  
		Size: 13.8 MB (13848948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6fc796e2e4e8dcc4413f98eb9ec637b3712c2d926f3eb799da1fa22e26f426`  
		Last Modified: Thu, 09 Feb 2023 09:32:55 GMT  
		Size: 4.4 MB (4399218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
