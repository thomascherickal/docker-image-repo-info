## `clojure:temurin-17-tools-deps-alpine`

```console
$ docker pull clojure@sha256:158dad59caa482429608aeb104134500ec9fce2924344c3efe5dabab4e9c855e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:b4fc02e3b182001cc1442f45e70fcbbf6d6d97a36a2e0204fff0762c0a77c403
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234520514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e01f3b166a88cd4e134a4df24afab00fce7d6085a901ec8b4c3f2b7b18fd887`
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
# Wed, 29 Mar 2023 19:50:07 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 29 Mar 2023 19:50:17 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0df7c1a58debee2668931ba4a07cb642475b23a5c61473761b6f293eba7c024a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 29 Mar 2023 19:50:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 29 Mar 2023 19:50:20 GMT
CMD ["jshell"]
# Mon, 17 Apr 2023 22:24:45 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:24:45 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:24:50 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Mon, 17 Apr 2023 22:24:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:24:50 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 22:24:50 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 22:24:50 GMT
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
	-	`sha256:447fb591121b7b0c1f352bc4baf3b7c840dcf32615f5b8504a4882e9048f2dca`  
		Last Modified: Wed, 29 Mar 2023 19:53:34 GMT  
		Size: 191.8 MB (191793866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cdd4cdb2078d3e1d61a38f6f6378966a085bf96adceecceeaffa29922faedb`  
		Last Modified: Wed, 29 Mar 2023 19:53:21 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d951f33cc04e52723a2bc34b10b9079a8dea70db1ee7e8559c60d0863087c42`  
		Last Modified: Mon, 17 Apr 2023 22:31:58 GMT  
		Size: 27.3 MB (27331282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304f43054ae060b711e8bc612c9ac8b57ad0395473a25a34f80f5d57ccc8638c`  
		Last Modified: Mon, 17 Apr 2023 22:31:56 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268a91b7f1a6bdfc9d0aee743e6b9f3bad865a0ec1ae11e3a924eaa9003f02ff`  
		Last Modified: Mon, 17 Apr 2023 22:31:56 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
