## `clojure:tools-deps-1.11.1.1155-alpine`

```console
$ docker pull clojure@sha256:39c4abcf0e2afc3fc02e70d0b2751cbfa6ebd2be6b89f6c567714d67f9a44c33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:tools-deps-1.11.1.1155-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:722ace771bac6ef125c99612bf9413c5fdda43dd30a50de475125e6a6a9dbe2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.4 MB (236398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cf7770598912abd21429f56605b93b06715c80068027504a3540d0b47247171`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

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
# Wed, 24 Aug 2022 19:21:34 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 24 Aug 2022 19:21:58 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1a1706304c26da0d8d2e05127c5aa7dba00e5401b2c0228c8ae894d2812beee0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Wed, 24 Aug 2022 19:22:01 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:22:01 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:54:04 GMT
ENV CLOJURE_VERSION=1.11.1.1155
# Wed, 24 Aug 2022 21:54:04 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:54:08 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7eb9aa2ecc6c0abfdb1578d4b99ca7c2055111aafa38524a12a6fb76fe01f30b *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 24 Aug 2022 21:54:09 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 24 Aug 2022 21:54:09 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 21:54:09 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 21:54:09 GMT
CMD ["-M" "--repl"]
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
	-	`sha256:baeea62e55107d5bcc912b1129b9a5e2551f65b996d4b613a8293615d39d04f4`  
		Last Modified: Wed, 24 Aug 2022 19:28:44 GMT  
		Size: 191.5 MB (191455735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf13604fb49c89ab5f868ccdf7c54522e7dd3f0639fc4e927a8c49026f1304`  
		Last Modified: Wed, 24 Aug 2022 19:28:29 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e54491df58e5eb33f9d1f23abb7d2981ced5c16313f03fe100012954595465b`  
		Last Modified: Wed, 24 Aug 2022 22:01:59 GMT  
		Size: 30.1 MB (30085164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556db2e657700045f07841fc2bcc518a82fb14a165f3646b1868bc5f6a043f53`  
		Last Modified: Wed, 24 Aug 2022 22:01:57 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638a210af4a8badbf5e92ddebed1cb03f53a0825981f6e3c52d9bc56366ffee1`  
		Last Modified: Wed, 24 Aug 2022 22:01:56 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
