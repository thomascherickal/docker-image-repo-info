## `eclipse-temurin:17-jre-alpine`

```console
$ docker pull eclipse-temurin@sha256:984703da8353d0a33eb04944b56665e84c6271e5d4f8a679e73cb5bd2b846301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:17-jre-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:cba04f7101096852719a1530feffbb04a232765a8180b083f6182bafc6b3e1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63398514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d5a7235045b27a97d729cfdbecc30a9ef2b654a36199106c3e1fb26a564b8ea`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

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
# Mon, 30 Oct 2023 23:26:31 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:29:01 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='70e5d108f51ae7c7b2435d063652df058723e303a18b4f72f17f75c5320052d3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_alpine-linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:29:02 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:29:02 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:29:02 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
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
	-	`sha256:2e50545f74853b08e46de79fa9fd930e933e5f42b830475459f2d49d2eede1fe`  
		Last Modified: Mon, 30 Oct 2023 23:37:20 GMT  
		Size: 46.9 MB (46854633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bee30a4e26167afdbec0760dcf442c666906f0383b8506c1115c3432e55c30`  
		Last Modified: Mon, 30 Oct 2023 23:37:14 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14d30cdf30f15457bf4df3b7d11fb0e15941339fc60431f5c96fd2863882e3`  
		Last Modified: Mon, 30 Oct 2023 23:37:14 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
