## `clojure:temurin-17-lein-2.9.8-alpine`

```console
$ docker pull clojure@sha256:d6a40b68a23c9b9595d6d6987666598b560469e873748e2df8fe67284f928b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-lein-2.9.8-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:4633d203a93d55dedb20cd2ce474dc147c9f2c255e407aedd2fcd851c46da555
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211805148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be69fd775b97068b09748ab5b1f779773c47c9a01a398ae47745dbdd85ce1944`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:55:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 08 Jun 2022 18:20:30 GMT
RUN apk add --no-cache libretls musl-locales musl-locales-lang tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 08 Jun 2022 18:22:03 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 08 Jun 2022 18:22:17 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5cbaece6aec44f6d3911cfa3c5a8659889e85042aff214c944c5fa1b5938a5fc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 08 Jun 2022 18:22:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Jun 2022 18:22:19 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 08 Jun 2022 18:22:19 GMT
CMD ["jshell"]
# Wed, 08 Jun 2022 19:04:34 GMT
ENV LEIN_VERSION=2.9.8
# Wed, 08 Jun 2022 19:04:34 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 08 Jun 2022 19:04:34 GMT
WORKDIR /tmp
# Wed, 08 Jun 2022 19:04:41 GMT
RUN set -eux; apk add --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Wed, 08 Jun 2022 19:04:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 08 Jun 2022 19:04:42 GMT
ENV LEIN_ROOT=1
# Wed, 08 Jun 2022 19:04:46 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 08 Jun 2022 19:04:46 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 08 Jun 2022 19:04:46 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 08 Jun 2022 19:04:46 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611b459a9f120c9f22143fbef6dda47c621957b1c86d4cbdf8fe3d9c762d728`  
		Last Modified: Wed, 08 Jun 2022 18:25:04 GMT  
		Size: 430.4 KB (430445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b675003cef6d41754d8984fa5998377cd14cb310f6d34d51d3105e9572af398`  
		Last Modified: Wed, 08 Jun 2022 18:26:48 GMT  
		Size: 191.8 MB (191809203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29402433809ae92da2b8604813d0a262eff1bdf9a6d1120c927de504e14e1a`  
		Last Modified: Wed, 08 Jun 2022 18:26:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b3ec612172bcf4cf659d1bf280b860cd1393c6d593bfc99eb2c7a14d1862df`  
		Last Modified: Wed, 08 Jun 2022 19:08:35 GMT  
		Size: 12.5 MB (12543159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5580ae9de2680306e7e97433e516ffe3080d5a162dfee6081630ed6af8528c5e`  
		Last Modified: Wed, 08 Jun 2022 19:08:35 GMT  
		Size: 4.2 MB (4207218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcab72b79eb47beec557ca07e08009c142b77b4cbc3f1fe1f2746e67153c597a`  
		Last Modified: Wed, 08 Jun 2022 19:08:34 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
