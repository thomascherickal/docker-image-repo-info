## `clojure:temurin-18-lein-2.9.8-alpine`

```console
$ docker pull clojure@sha256:8ac659e41729b79c123a175a9ffe0aa1af65050391a8561cb692827eae0480f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-18-lein-2.9.8-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:f093bef0b07c240617deff223653835a52856b040ceca07b6c9c18e8dc004b35
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.9 MB (212858497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf024a5964db02e2f76cea6a8cdfef753c1fb326ff864f45ab9af2028fc300b`
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
# Wed, 08 Jun 2022 18:22:46 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 08 Jun 2022 18:23:06 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ab72b28e1ce896e6b11e2b362c12c36007ebe9963d8954bc11e637be1f024dfe';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_alpine-linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 08 Jun 2022 18:23:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Jun 2022 18:23:07 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 08 Jun 2022 18:23:07 GMT
CMD ["jshell"]
# Wed, 08 Jun 2022 19:05:55 GMT
ENV LEIN_VERSION=2.9.8
# Wed, 08 Jun 2022 19:05:55 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 08 Jun 2022 19:05:55 GMT
WORKDIR /tmp
# Wed, 08 Jun 2022 19:06:01 GMT
RUN set -eux; apk add --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Wed, 08 Jun 2022 19:06:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 08 Jun 2022 19:06:01 GMT
ENV LEIN_ROOT=1
# Wed, 08 Jun 2022 19:06:05 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Wed, 08 Jun 2022 19:06:06 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 08 Jun 2022 19:06:06 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 08 Jun 2022 19:06:06 GMT
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
	-	`sha256:a4999eef7250c59af1e8ce612900661002c5085eced42d5c29d3c1d0aa438775`  
		Last Modified: Wed, 08 Jun 2022 18:27:39 GMT  
		Size: 192.9 MB (192862537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262edfdf635ac957aea206f1847f59984d074da776116ffbfaadedb1b331f18b`  
		Last Modified: Wed, 08 Jun 2022 18:27:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0d43dd35ae347034986dde5fb35e1fcd586962526a99ce9edfb101192c2e8f`  
		Last Modified: Wed, 08 Jun 2022 19:09:33 GMT  
		Size: 12.5 MB (12543167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9142269e91a3a8582cae6b410c00cca32c512a222921d40d48a3cc36ecccf4f`  
		Last Modified: Wed, 08 Jun 2022 19:09:32 GMT  
		Size: 4.2 MB (4207224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d2bed6c743cb697b4d6d4820bc88bc4902f96e8fe17482c3f345f364e58468`  
		Last Modified: Wed, 08 Jun 2022 19:09:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
