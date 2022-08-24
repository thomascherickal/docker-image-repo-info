## `clojure:temurin-17-lein-alpine`

```console
$ docker pull clojure@sha256:43a0387e9596182d170053cbca3338645f325ce704ebbff40f1a95f3213068fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-lein-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:ab5d3a43b86fcebefa552fde89a154dbd6f1dd05fde87dda2b86322ddf9424f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223594558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0920c218c4759dce8cae9600aa4e2a0839c2a0bbb62a0e1b78cb3ab0d87bd22c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 19:19:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:19:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:19:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:19:40 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 24 Aug 2022 19:21:34 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 24 Aug 2022 19:21:58 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1a1706304c26da0d8d2e05127c5aa7dba00e5401b2c0228c8ae894d2812beee0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 24 Aug 2022 19:22:01 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:22:01 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:53:04 GMT
ENV LEIN_VERSION=2.9.10
# Wed, 24 Aug 2022 21:53:04 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 21:53:04 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:53:14 GMT
RUN set -eux; apk add --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Wed, 24 Aug 2022 21:53:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 21:53:14 GMT
ENV LEIN_ROOT=1
# Wed, 24 Aug 2022 21:53:16 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 24 Aug 2022 21:53:17 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 21:53:17 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 21:53:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107abfa4a9656cc98051eebaf02de090526191f4d53ab3733605b34f84513224`  
		Last Modified: Thu, 11 Aug 2022 19:29:52 GMT  
		Size: 12.1 MB (12050073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baeea62e55107d5bcc912b1129b9a5e2551f65b996d4b613a8293615d39d04f4`  
		Last Modified: Wed, 24 Aug 2022 19:28:44 GMT  
		Size: 191.5 MB (191455735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf13604fb49c89ab5f868ccdf7c54522e7dd3f0639fc4e927a8c49026f1304`  
		Last Modified: Wed, 24 Aug 2022 19:28:29 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77427ed5d8f87dbd00b82036a022d86cc6f26d07915257a7e04f913c20f94f25`  
		Last Modified: Wed, 24 Aug 2022 22:01:00 GMT  
		Size: 12.9 MB (12883444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5c6390a37f411f04589354f330135003ae63e336806ef515f34758152d94b8`  
		Last Modified: Wed, 24 Aug 2022 22:01:00 GMT  
		Size: 4.4 MB (4398671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5291868e45c607c933baa72f17c2d363cfa80c0b150d3091a7ce6673a136c0e4`  
		Last Modified: Wed, 24 Aug 2022 22:00:59 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
