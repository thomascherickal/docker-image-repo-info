## `eclipse-temurin:21-alpine`

```console
$ docker pull eclipse-temurin@sha256:001dfe1c179b3f315bd6549ad1fe94fd7204984319bd3c0f3b385b5188cb18b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `eclipse-temurin:21-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:76163bd4f26586627c4257472f7115d7e9b1d9e05cca2b33b36b7d358316c366
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.2 MB (174208885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74024acf447190e0b1cc02c972ed6546b992ee2884842a64b2b99702f5586c3b`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 02:50:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 19 Oct 2023 02:50:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 02:50:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:26:31 GMT
RUN set -eux;     apk add --no-cache         bash         fontconfig ttf-dejavu         java-cacerts         libretls zlib         musl-locales musl-locales-lang         binutils         tzdata     ;     rm -rf /var/cache/apk/*
# Mon, 30 Oct 2023 23:29:38 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:29:47 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='77006c0a753808c2a6662007906eb6eb230f2fb6eb9d201a39cc46113e68f82c';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_aarch64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|x86_64)          ESUM='422f23f5109056cacb9227247bebf8532e2dc3c9d505e71637ba610569d6b3ff';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:29:49 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:29:49 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:29:49 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 30 Oct 2023 23:29:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3c4df72d74e9b84f1215596adc1b562a87b2c2bd9249ba1433455079b00218`  
		Last Modified: Mon, 30 Oct 2023 23:35:19 GMT  
		Size: 13.1 MB (13141022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557d0e6d84070f1613c688db633bc297fea0a029d3a22d4fe738533f232c1d43`  
		Last Modified: Mon, 30 Oct 2023 23:38:41 GMT  
		Size: 157.7 MB (157664989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b015da0bc5f29d7e54638ef2c9b6621d293e70c697f7a84d606b0c468ad4bbb9`  
		Last Modified: Mon, 30 Oct 2023 23:38:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae9403a54ca68efac5723aeaa16e4f4fb7045e4d0fa413ee823194acd675092`  
		Last Modified: Mon, 30 Oct 2023 23:38:29 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:21-alpine` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:11e45ed57b9bc892034476e315b0b8067949171874fe97a1d0da8577ec43b9cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172522125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb7129b00e6324ebcd28341854cd17bb8750943ee8b828831083f3d6482a2f5`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:06:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 19 Oct 2023 03:06:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Oct 2023 03:06:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:45:52 GMT
RUN set -eux;     apk add --no-cache         bash         fontconfig ttf-dejavu         java-cacerts         libretls zlib         musl-locales musl-locales-lang         binutils         tzdata     ;     rm -rf /var/cache/apk/*
# Mon, 30 Oct 2023 23:45:52 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:46:01 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='77006c0a753808c2a6662007906eb6eb230f2fb6eb9d201a39cc46113e68f82c';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_aarch64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|x86_64)          ESUM='422f23f5109056cacb9227247bebf8532e2dc3c9d505e71637ba610569d6b3ff';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:46:04 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:46:04 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:46:04 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 30 Oct 2023 23:46:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb307395b9c465620415149d03a302b3b0b883166dde912aca3bba924bfeea3`  
		Last Modified: Mon, 30 Oct 2023 23:52:47 GMT  
		Size: 13.5 MB (13515517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c8e0a9c6608bf9e2b6937fb2e1ee9990fd7819a48cbd3cadfef2ad692769c7`  
		Last Modified: Mon, 30 Oct 2023 23:52:56 GMT  
		Size: 155.7 MB (155673871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f85d1edfcd3f467ec3939e5300b8cb2ee886fea32e5e48e3a54142c7775a647`  
		Last Modified: Mon, 30 Oct 2023 23:52:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79254b79d8abf76e6fa27de9908f04f3ab0b347e2caa9fa13d72270403ce4072`  
		Last Modified: Mon, 30 Oct 2023 23:52:46 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
