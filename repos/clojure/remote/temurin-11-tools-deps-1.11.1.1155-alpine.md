## `clojure:temurin-11-tools-deps-1.11.1.1155-alpine`

```console
$ docker pull clojure@sha256:b6d6f875499aa25da7ac73826eed0b3b4411f6212c1be621a4c38a055c8d3891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-tools-deps-1.11.1.1155-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:ba9da182efaa4c507c4184e92440225aa05cf3135c7fc5c90c40a54e7b1a32b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.4 MB (238399801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c869652de2af47b5d1ca35ed3908d1b8ae8c771f8ab2623020b57cc070b82d`
-	Default Command: `["clj"]`

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
# Wed, 24 Aug 2022 19:19:58 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:20:14 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='327b3bfd1c14e15bf6c7fb4d0c6c3f9406c1282a16e24b1424215d764f687cb6';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 24 Aug 2022 19:20:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:20:17 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:51:15 GMT
ENV CLOJURE_VERSION=1.11.1.1155
# Wed, 24 Aug 2022 21:51:15 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:51:20 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7eb9aa2ecc6c0abfdb1578d4b99ca7c2055111aafa38524a12a6fb76fe01f30b *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 24 Aug 2022 21:51:20 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 24 Aug 2022 21:51:21 GMT
CMD ["clj"]
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
	-	`sha256:29496409cb750e4cd34c0abc2a0af5d4a8c9983eb3a8de05281f672289d5fb1e`  
		Last Modified: Wed, 24 Aug 2022 19:25:48 GMT  
		Size: 193.5 MB (193457720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0469b5bbda2d25b40afdbe052d9452b8af0246a6fc7abcea846b5ff7512de5b8`  
		Last Modified: Wed, 24 Aug 2022 19:25:34 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abeec68a4395e60e713953a4743e06c7f1acf0d3ca31a5bbf34072541f9ef69`  
		Last Modified: Wed, 24 Aug 2022 21:58:55 GMT  
		Size: 30.1 MB (30085150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f349d5ff70ec227b44d83ac9be75d5b2e06255a10305293765b5ea8b4b4553`  
		Last Modified: Wed, 24 Aug 2022 21:58:53 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
