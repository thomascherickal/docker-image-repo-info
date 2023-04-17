## `clojure:temurin-8-tools-deps-alpine`

```console
$ docker pull clojure@sha256:8bf72ddb279fbef55aef0942a1746ab1ca8f54062c2612ffe50d2395673697a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:a506b348e2514c1b0c8ee10af42a291d70f08fa895cfa41c2d3a1840cb96e7b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95267683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b16c2685954c872d627d61ed2b12d5b86adb5c34294d09c2474588d3d6e6554`
-	Default Command: `["clj"]`

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
# Wed, 29 Mar 2023 19:48:58 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Wed, 29 Mar 2023 19:49:03 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='389c0d2ea59742103f46f1dd6d2c83e43e9f935f3f0485b1f9e74ac4e8c5ce47';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 29 Mar 2023 19:49:04 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Mon, 17 Apr 2023 22:20:45 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:20:45 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:20:50 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Mon, 17 Apr 2023 22:20:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:20:50 GMT
CMD ["clj"]
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
	-	`sha256:2b41571bb2675b142d9a5fdbff0ee09d26c687e3e6df9d09f437f3909fecf98a`  
		Last Modified: Wed, 29 Mar 2023 19:52:08 GMT  
		Size: 52.5 MB (52541504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36ccf21b1cfec1e8554234a199d876fdc59f6a3906c4806eca7022fd312ea28`  
		Last Modified: Wed, 29 Mar 2023 19:52:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b0185d42b0bf346873b1a1bddccd66cf21b1ffdb6ff4e552ffb3ebe1b8766d`  
		Last Modified: Mon, 17 Apr 2023 22:28:48 GMT  
		Size: 27.3 MB (27331230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e237208b8aedcfb67daade8258124cce8a2b92c93b7905505ae1d3ec52f54d`  
		Last Modified: Mon, 17 Apr 2023 22:28:46 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
