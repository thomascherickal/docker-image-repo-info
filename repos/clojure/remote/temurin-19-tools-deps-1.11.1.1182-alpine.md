## `clojure:temurin-19-tools-deps-1.11.1.1182-alpine`

```console
$ docker pull clojure@sha256:150eb0dedc8e94139cc84657851e8356a2e4c212842e6610f960ff10f7d8112f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-19-tools-deps-1.11.1.1182-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:c531e4ef9614950e51e0a97c1b9d96205a5f3892d8e532e6ba0d8546edc926f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.0 MB (244973294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d820be688fa8102d587976435d31f38695dcae44bbfc747361b02f2bffa80f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 16:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 07 Oct 2022 16:53:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 16:53:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Oct 2022 16:53:21 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Fri, 07 Oct 2022 16:55:27 GMT
ENV JAVA_VERSION=jdk-19+36
# Fri, 07 Oct 2022 16:55:46 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='2a073c3cc977317baf7c0c4995be38d33e3ed74e9fa4ac075933016e68f18252';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19%2B36/OpenJDK19U-jdk_x64_alpine-linux_hotspot_19_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Fri, 07 Oct 2022 16:55:49 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 07 Oct 2022 16:55:49 GMT
CMD ["jshell"]
# Fri, 28 Oct 2022 20:40:12 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:40:12 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:40:18 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Fri, 28 Oct 2022 20:40:18 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:40:18 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:40:18 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:40:18 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5835cc7e6eb64b728c9694dd72d8aede877af0a2ec44f981847853af9abbf5`  
		Last Modified: Fri, 07 Oct 2022 16:57:51 GMT  
		Size: 12.0 MB (12041341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862e44a33ca79d5a7f3c2c7f6721a8c1ca58d24fb209c1cac5ca9a61c3902ce`  
		Last Modified: Fri, 07 Oct 2022 17:00:32 GMT  
		Size: 200.0 MB (200041295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6cbbd4fbc13d9b25eb5ece2353108b5979269f23f7bccb805f72feaf03bf66`  
		Last Modified: Fri, 07 Oct 2022 17:00:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036f6042a0a836dda2f5b84af1d5c23a8eeca2ce156e08bf3159785255f91cdc`  
		Last Modified: Fri, 28 Oct 2022 20:50:58 GMT  
		Size: 30.1 MB (30083401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5524b7c6a4d8ccd0240eab0c466c9112b27b7dcc5f5a37a0e76e56d9df52675c`  
		Last Modified: Fri, 28 Oct 2022 20:50:55 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850e8b9a055a9e70f27e5f895d4f04b624e72f1ec548163509f3722237c1637c`  
		Last Modified: Fri, 28 Oct 2022 20:50:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
