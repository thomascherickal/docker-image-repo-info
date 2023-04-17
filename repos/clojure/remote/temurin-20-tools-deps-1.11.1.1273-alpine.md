## `clojure:temurin-20-tools-deps-1.11.1.1273-alpine`

```console
$ docker pull clojure@sha256:6a46a267a4a0bb838d888fbc37ad2c4187bb2726ed5a7944918ff55e74e5c02f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-20-tools-deps-1.11.1.1273-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:0b25362ab0fe87e7b60d98457589fff76dcc092a6c0618e5488a25186a2b536c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.7 MB (244664632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce21a8a348b76eea3926a79c02b43abb0e270f7399433927df84279fcec4596f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:48:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 29 Mar 2023 19:48:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:48:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 29 Mar 2023 19:48:58 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 29 Mar 2023 19:50:43 GMT
ENV JAVA_VERSION=jdk-20+36
# Wed, 29 Mar 2023 19:50:54 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='328c8cbfe3433a4556f68329323c671929bd9082b1113fa8a87892a1b1563ec7';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jdk_x64_alpine-linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 29 Mar 2023 19:50:57 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 29 Mar 2023 19:50:57 GMT
CMD ["jshell"]
# Mon, 17 Apr 2023 22:26:16 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:26:16 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:26:21 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Mon, 17 Apr 2023 22:26:21 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:26:21 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 22:26:21 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 22:26:21 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ed194273be4d4d02a2158c3e7c9ea96095ed70f65939d53f4968b0f225c628`  
		Last Modified: Wed, 29 Mar 2023 19:52:03 GMT  
		Size: 12.0 MB (12019605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3633cf7f956a62f51da6f31e93ff252b4ba9a0c47c8c5ff9b0e4e67e86d2926`  
		Last Modified: Wed, 29 Mar 2023 19:54:18 GMT  
		Size: 201.9 MB (201938032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce69eafe6a9e350ee48a47add689bb976296149c1dd5250e6700bb16029e25af`  
		Last Modified: Wed, 29 Mar 2023 19:54:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb466f8dbe006a6f70d95a170b117e43bffd8d48e796d2d2e144bf2b116c4126`  
		Last Modified: Mon, 17 Apr 2023 22:33:44 GMT  
		Size: 27.3 MB (27331230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a3c3fe2355284b84ae0ba0827de040d842e8c43426b5a1bb9ecb72ed351bc9`  
		Last Modified: Mon, 17 Apr 2023 22:33:42 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2a077d01e4afc334118c679f41a461d844054707e55ff7d7739bd53611ccb`  
		Last Modified: Mon, 17 Apr 2023 22:33:43 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
