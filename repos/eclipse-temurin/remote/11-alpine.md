## `eclipse-temurin:11-alpine`

```console
$ docker pull eclipse-temurin@sha256:0f42a9544bb88d43ce43e6668cf52423951099e14761d35779d0175414f0dd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eclipse-temurin:11-alpine` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:fd3753e16935cf54faebd41b5e0167c7385d47fe8f5c983c051fe04e0748c895
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153164076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b582f04be5a8e22a60e8fbaf2e99f641a8f180761c63177d79cac2206fe54f`
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
# Mon, 30 Oct 2023 23:22:37 GMT
RUN set -eux;     apk add --no-cache         bash         fontconfig ttf-dejavu         java-cacerts         libretls zlib         musl-locales musl-locales-lang         tzdata     ;     rm -rf /var/cache/apk/*
# Mon, 30 Oct 2023 23:22:38 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:22:46 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d5e2235d3707526f7c9ba3f0dc194e60d5dec33eceff2a2dcf9d874464cc0e9e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:22:48 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:22:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:22:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 30 Oct 2023 23:22:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02a3a37ba0a441c23edb967d901e4af5b508796b983fbb71e14ad89db9a9999`  
		Last Modified: Mon, 30 Oct 2023 23:32:06 GMT  
		Size: 9.3 MB (9276545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12e67e82faf020e769d46cccfc7f1620ccb86e04b4576b070512194641eb854`  
		Last Modified: Mon, 30 Oct 2023 23:32:15 GMT  
		Size: 140.5 MB (140484655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43caa4ccd4f85f364bbf72014cc960dc6fb6703350eceaee77976cf6313c8a55`  
		Last Modified: Mon, 30 Oct 2023 23:32:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8800858de447fac23faff681df1122b67d784efb0ee850d3d9551bcb5e9b19f8`  
		Last Modified: Mon, 30 Oct 2023 23:32:04 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
