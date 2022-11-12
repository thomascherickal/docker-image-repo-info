## `clojure:temurin-11-boot-alpine`

```console
$ docker pull clojure@sha256:97bca2bf710ded1bd723c51ce461203a4f53c00e65f282ecb988f7fa052f3793
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:df65734f2d81a5caa33dd4445bcd20fdd21d16de481e1871a128f13a89427820
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.3 MB (268329196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f4cc5304f2a9019ccf9967494ca97d9603a67b0c268bac4c7d0c12c8a60883`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:12:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 12 Nov 2022 05:12:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Nov 2022 05:12:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 12 Nov 2022 05:12:06 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Sat, 12 Nov 2022 05:12:49 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Sat, 12 Nov 2022 05:13:02 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='774d5955c09893dda14e3eb0fd3e239a6b2cec58615fcf4ec68747260b6e1cc1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Sat, 12 Nov 2022 05:13:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 12 Nov 2022 05:13:05 GMT
CMD ["jshell"]
# Sat, 12 Nov 2022 10:33:51 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 12 Nov 2022 10:33:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 12 Nov 2022 10:33:51 GMT
WORKDIR /tmp
# Sat, 12 Nov 2022 10:33:53 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Sat, 12 Nov 2022 10:33:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 12 Nov 2022 10:33:53 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 12 Nov 2022 10:34:39 GMT
RUN boot
# Sat, 12 Nov 2022 10:34:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9822f87bb1185b1d8f81aa09fc8a20796bb3db4c90da28c6177e0fd8a3d8d3`  
		Last Modified: Sat, 12 Nov 2022 05:16:37 GMT  
		Size: 12.0 MB (12030631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec5de7441ae3d196472e565fe52f43eb0e27b60813e788d87440a3578ca867d`  
		Last Modified: Sat, 12 Nov 2022 05:17:32 GMT  
		Size: 193.8 MB (193812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0dd61568d72d7bb5ed1797c90e222d6e5cd711c8339a9672cbf0a94378b103`  
		Last Modified: Sat, 12 Nov 2022 05:17:18 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af20cd366109918204a6dc56e6c96771fc5ee450f3c9f467c87a3c95f49284f`  
		Last Modified: Sat, 12 Nov 2022 10:41:25 GMT  
		Size: 858.7 KB (858656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0464a0f472e9d5d6824d8a26602a4c93570b65576872e8fd571b2c3c9858b4f`  
		Last Modified: Sat, 12 Nov 2022 10:41:28 GMT  
		Size: 58.8 MB (58820970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
