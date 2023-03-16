## `clojure:temurin-19-tools-deps-1.11.1.1257-alpine`

```console
$ docker pull clojure@sha256:4e598b8938970c3062b0ae1d444ea836487f8793242ea0315fc54d5c25096e96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-19-tools-deps-1.11.1.1257-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:f1f1fe54596b92ec8b4b22974e4d5468b5ca59ce77b3a282d19010cb7671da81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.0 MB (243030289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1784a407cdd5ef7087848f62796f575c2cf8534b1910a8736ad7091e1e96c14`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:24:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 11 Feb 2023 05:24:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:24:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 11 Feb 2023 05:24:09 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Sat, 11 Feb 2023 05:26:26 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Sat, 11 Feb 2023 05:26:49 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e2d971400ad2db25ad43ea6fa2058b269c0236e3977986dcdee2097da301beb2';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_alpine-linux_hotspot_19.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Sat, 11 Feb 2023 05:26:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 11 Feb 2023 05:26:51 GMT
CMD ["jshell"]
# Thu, 16 Mar 2023 20:26:29 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 16 Mar 2023 20:26:29 GMT
WORKDIR /tmp
# Thu, 16 Mar 2023 20:26:34 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Thu, 16 Mar 2023 20:26:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 16 Mar 2023 20:26:34 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 16 Mar 2023 20:26:34 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 16 Mar 2023 20:26:34 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55337210c571172bc884a7dfb6dc597adab6b6ef741c06ca3200884ffc4b2b`  
		Last Modified: Sat, 11 Feb 2023 05:28:55 GMT  
		Size: 12.0 MB (12020168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179e78b7ac3beb399f002d9c566af29327c2fd2ac6956665f64f53aecf8d1119`  
		Last Modified: Sat, 11 Feb 2023 05:31:21 GMT  
		Size: 200.3 MB (200308729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ece7618d1e8c49aa5ff521f5133d9ab5bd61543cfe7493b40e99d10a2ec5d6`  
		Last Modified: Sat, 11 Feb 2023 05:31:05 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecbaac11eb8b2970a16c26918bd6cf3b688c782c10dbdd4991ebd7e81a87199`  
		Last Modified: Thu, 16 Mar 2023 20:37:02 GMT  
		Size: 27.3 MB (27325740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4414115773e8a22fa8de9e9f1f068658087aba87403f584b212e1e5353a916b0`  
		Last Modified: Thu, 16 Mar 2023 20:37:00 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785f1c9838cef79bd9ef2983bfa331413411d8f6b407c901d58ed1895a0637ed`  
		Last Modified: Thu, 16 Mar 2023 20:37:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
