## `eclipse-temurin:21-jre-alpine`

```console
$ docker pull eclipse-temurin@sha256:2a4755c16fe3390e6a89daed9adfc6d9dc7be116dfce84497cf84f761b973311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `eclipse-temurin:21-jre-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:6b990458235e07c018abfc2d21f6f284789e3f97cf542402ad226b3724d8ea7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69651770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645c1bf95327b6da1f574c3215f04ab8f47b92bdfb228593ad92e2fdec309f78`
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
# Mon, 30 Oct 2023 23:29:38 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:30:26 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2898ea1ddf6f70f09b09cf99d928f6d4c862f78f81104f5dce3e44a832b8444a';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jre_aarch64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|x86_64)          ESUM='a8fcc43927664ba191c9a77d1013f1f32fec1acc22fe6f0c29d687221f2cc95d';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jre_x64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:30:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:30:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:30:27 GMT
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
	-	`sha256:7e53c664d1ad8d93ebe74f0c8ce9e83c1af21e4ffc62d673684686c8389bc861`  
		Last Modified: Mon, 30 Oct 2023 23:39:47 GMT  
		Size: 53.1 MB (53107888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5648fe788e03429688be53b769e2e1655f9a5742c41f292de712717111cba9`  
		Last Modified: Mon, 30 Oct 2023 23:39:40 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06d2969233a3c78bcc756a87424372bc2b3ebc6c97ef1a7f1e63c42cfe7d51b`  
		Last Modified: Mon, 30 Oct 2023 23:39:40 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:21-jre-alpine` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:7d347974dbaa4354f9fb1de85152147220d1589bc0d00767e52b0de53641f194
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69026613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ceefc759fe1b19b2b5e2e318095fbb0c3a7382446945da45efbdb196f9de93`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

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
# Mon, 30 Oct 2023 23:46:37 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2898ea1ddf6f70f09b09cf99d928f6d4c862f78f81104f5dce3e44a832b8444a';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jre_aarch64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        amd64|x86_64)          ESUM='a8fcc43927664ba191c9a77d1013f1f32fec1acc22fe6f0c29d687221f2cc95d';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jre_x64_alpine-linux_hotspot_21.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:46:38 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:46:38 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:46:38 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
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
	-	`sha256:e0d2bc3f16aef3fd0c117b4734ca2d27d5ae3dba83147c7912cab44c4b2bb10f`  
		Last Modified: Mon, 30 Oct 2023 23:53:58 GMT  
		Size: 52.2 MB (52178372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f468a40be64b934faa77228ebdce3ffbe650c81c7cd861cd1676c348ee03be`  
		Last Modified: Mon, 30 Oct 2023 23:53:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93fdb6764feb15842dba4111b9236aacb1fd0f76a2bf942aa9d18e1fc041a33`  
		Last Modified: Mon, 30 Oct 2023 23:53:52 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
