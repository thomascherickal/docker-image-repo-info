## `clojure:temurin-8-tools-deps-alpine`

```console
$ docker pull clojure@sha256:9e576a21d0e6cf2eed13b009fbb1045ba540ecfcdd03671a4a6aab26f6dfdba0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:ff7787b9945cc5a515f95a81ff7e0ea80b166a991cb4c1f2885c180cf8982eac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.6 MB (91624314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca21ccbf40e550e6610e1a101ee2f8c25ecc46316a12f5621c74065e9c59fc8e`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 24 May 2023 23:34:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 24 May 2023 23:34:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 23:34:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 24 May 2023 23:34:29 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 24 May 2023 23:34:29 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 24 May 2023 23:34:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='cfdf8e07c8eeb087b7a2895b90fc0a19986bcff85006f1e2b708e3964909aa8e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_alpine-linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 24 May 2023 23:34:36 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 24 May 2023 23:56:48 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Wed, 24 May 2023 23:56:48 GMT
WORKDIR /tmp
# Wed, 24 May 2023 23:56:53 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 24 May 2023 23:56:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 24 May 2023 23:56:53 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdde4a302e0d0ee2ef6760bf84344d762835ef2d38d2a1a1062c7d038fe2615b`  
		Last Modified: Wed, 24 May 2023 23:37:36 GMT  
		Size: 7.6 MB (7648427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d694a2b7c16a77c50982c0d6c082b7283771de0ec5cc847bd355b7ab684aedc9`  
		Last Modified: Wed, 24 May 2023 23:37:40 GMT  
		Size: 52.5 MB (52539524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d54ff8e92ad62b25089a5c48736e5c228115778e74dc2155361eda232c376ae`  
		Last Modified: Wed, 24 May 2023 23:37:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7ae14b515a7f9a478f354d18792afac6c4a3d68d046fe2e4a10829171ebdbb`  
		Last Modified: Thu, 25 May 2023 00:00:34 GMT  
		Size: 28.0 MB (28038091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d324785f34395c87c5d0c7d4856b80382dabb889a63e083401f5cb3a616548e6`  
		Last Modified: Thu, 25 May 2023 00:00:33 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
