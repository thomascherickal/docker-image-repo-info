## `tomcat:jre11-temurin-focal`

```console
$ docker pull tomcat@sha256:2a3c820b247c80bb12931ea1ac70e86a189bbe843449a0286c3310af710aaa05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre11-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:1b4c91761d7419bbc779592003e624163f2fb0c61d2272702e5ba9fab83f95ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100827598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3ce3e150296f6c1f11d06bb57b77be73b02f0ba21095a81abbf8888197c203`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:25:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 04:46:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:47:03 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Fri, 01 Oct 2021 04:47:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 01 Oct 2021 04:47:26 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 04:47:27 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 01 Oct 2021 08:58:36 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Oct 2021 08:58:36 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 08:58:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Oct 2021 08:58:37 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Oct 2021 08:58:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 08:58:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 08:58:38 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 01 Oct 2021 08:58:38 GMT
ENV TOMCAT_MAJOR=10
# Wed, 06 Oct 2021 19:15:07 GMT
ENV TOMCAT_VERSION=10.0.12
# Wed, 06 Oct 2021 19:15:07 GMT
ENV TOMCAT_SHA512=e084fc0cc243c0a9ac7de85ffd4b96d00b40b5493ed7ef276d91373fe8036bc953406cd3c48db6b5ae116f2af162fd1bfb13ecdddf5d64523fdd69a9463de8a3
# Wed, 06 Oct 2021 19:15:08 GMT
COPY dir:4e4cabf43e85825c572ae5d21bd3efda8950858cf53d467acf7422a156c0da29 in /usr/local/tomcat 
# Wed, 06 Oct 2021 19:15:12 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 19:15:14 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Oct 2021 19:15:15 GMT
EXPOSE 8080
# Wed, 06 Oct 2021 19:15:15 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfa0820368ab7e292075aa2118a674d9feccdeb45d31bfc0efa051af8683cc8`  
		Last Modified: Fri, 01 Oct 2021 04:49:34 GMT  
		Size: 16.0 MB (16033156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8604c4f12c97ba136102a9f98d44f3e02bc89c3ab66f4fc5e8195983bd07e8`  
		Last Modified: Fri, 01 Oct 2021 04:50:44 GMT  
		Size: 43.2 MB (43219899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9152c3f82ecdbd7c86979067f9019ee95a132a28ac6e532fb6847b438a59b6fe`  
		Last Modified: Fri, 01 Oct 2021 04:50:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12bcafdda20caf72322b09868c6a276f692d8ec9e182e04ddf34868f2f5fe1`  
		Last Modified: Fri, 01 Oct 2021 09:27:06 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fe17f562740f200bf1c5ad966fc33f38b410d278d5eec3ae4586e66319f467`  
		Last Modified: Wed, 06 Oct 2021 20:05:01 GMT  
		Size: 12.6 MB (12559485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edd751660257acdbd3dc5793cc5b8c3e6d6516ea233362d1fb202da1d830262`  
		Last Modified: Wed, 06 Oct 2021 20:05:00 GMT  
		Size: 445.7 KB (445679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a7f10c2e6f40a771db97bdc1f13f48e968bc51bf948d20d58a2911865f28ba`  
		Last Modified: Wed, 06 Oct 2021 20:04:59 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:53d5290395af3233b8f2d35eb75f932632d98c45211350e4b8b26e60db66c8a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93728139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbd049d60614873235cd677f83a0b77ac1c17bc4b06c83bd32b50663ffdae5af`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 23:26:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Oct 2021 23:26:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 23:28:04 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Sat, 02 Oct 2021 23:29:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 02 Oct 2021 23:29:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Oct 2021 23:29:22 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sun, 03 Oct 2021 03:31:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sun, 03 Oct 2021 03:31:06 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 03 Oct 2021 03:31:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sun, 03 Oct 2021 03:31:09 GMT
WORKDIR /usr/local/tomcat
# Sun, 03 Oct 2021 03:31:09 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sun, 03 Oct 2021 03:31:09 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sun, 03 Oct 2021 03:31:10 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Sun, 03 Oct 2021 03:31:10 GMT
ENV TOMCAT_MAJOR=10
# Wed, 06 Oct 2021 19:33:38 GMT
ENV TOMCAT_VERSION=10.0.12
# Wed, 06 Oct 2021 19:33:39 GMT
ENV TOMCAT_SHA512=e084fc0cc243c0a9ac7de85ffd4b96d00b40b5493ed7ef276d91373fe8036bc953406cd3c48db6b5ae116f2af162fd1bfb13ecdddf5d64523fdd69a9463de8a3
# Wed, 06 Oct 2021 19:33:41 GMT
COPY dir:73becd31355ed7984fd7be3a144455cfafebf3e657b33fca99fd4df65b3cdcb6 in /usr/local/tomcat 
# Wed, 06 Oct 2021 19:33:50 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 19:33:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Oct 2021 19:33:54 GMT
EXPOSE 8080
# Wed, 06 Oct 2021 19:33:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e2199de8cbbc437199cb30a504a0e04104b5a48bab3447d69fdb35ef7e9fd`  
		Last Modified: Sat, 02 Oct 2021 23:33:01 GMT  
		Size: 14.9 MB (14897772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1140eabca81e1b86f3e62211bd292832d44563461799468b5ed38e39c83944f8`  
		Last Modified: Sat, 02 Oct 2021 23:34:42 GMT  
		Size: 41.8 MB (41831607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e4d6efc1e2f53305a32b4de31e48c96033898b8d7ff215b498731405f7bf98`  
		Last Modified: Sat, 02 Oct 2021 23:34:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2e3c5bbfe03c4b8f4b0fb938dfa563187e0d8755684ff6dc14e4ba383482c7`  
		Last Modified: Sun, 03 Oct 2021 03:49:46 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680156f6245786101ca0e0d426280044574afe62f7217169b54805852bb39741`  
		Last Modified: Wed, 06 Oct 2021 19:47:11 GMT  
		Size: 12.5 MB (12508844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd4be2737e912fadb8d637eb80e0ce8c45431e85ff467aba7496643351f206a`  
		Last Modified: Wed, 06 Oct 2021 19:47:07 GMT  
		Size: 422.2 KB (422235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f735b511f8793dcb65f78b84a9ebaeb24005de24979e137cf506c7fdc7d72f98`  
		Last Modified: Wed, 06 Oct 2021 19:47:06 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:44822b6ad7445c30c0c7f97eef208d35ddf4a852ec0a6877b94a00fa15e58cc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.4 MB (97370642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d9095b254b31cbf70bfa4a76685c98594e88712378401b31e8dca981708bd01`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 03:29:40 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:30:14 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Fri, 01 Oct 2021 03:30:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 01 Oct 2021 03:30:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 03:30:40 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 13 Oct 2021 08:43:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 13 Oct 2021 08:43:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 08:43:31 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 13 Oct 2021 08:43:32 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Oct 2021 08:43:33 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 13 Oct 2021 08:43:34 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 13 Oct 2021 08:43:35 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 13 Oct 2021 08:43:36 GMT
ENV TOMCAT_MAJOR=10
# Wed, 13 Oct 2021 08:56:13 GMT
ENV TOMCAT_VERSION=10.0.12
# Wed, 13 Oct 2021 08:56:14 GMT
ENV TOMCAT_SHA512=e084fc0cc243c0a9ac7de85ffd4b96d00b40b5493ed7ef276d91373fe8036bc953406cd3c48db6b5ae116f2af162fd1bfb13ecdddf5d64523fdd69a9463de8a3
# Wed, 13 Oct 2021 08:56:16 GMT
COPY dir:04a5bf9d491f55c996a86d30110c7b5d25067e9c688ca0a9db55c4fb06e359dd in /usr/local/tomcat 
# Wed, 13 Oct 2021 08:56:21 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:56:22 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Oct 2021 08:56:23 GMT
EXPOSE 8080
# Wed, 13 Oct 2021 08:56:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a41a8557fe5edae6e15c9c361239e4a3156f9c03d105c51d28a42e3e13bc82`  
		Last Modified: Fri, 01 Oct 2021 03:33:27 GMT  
		Size: 15.9 MB (15895222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66816c95c6d7b51ddf32ebcfb5cb6866c55cccefa8ee6778b5484634d04c06e3`  
		Last Modified: Fri, 01 Oct 2021 03:34:51 GMT  
		Size: 41.5 MB (41518370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b883e9e1334cb8bb16423485c83f51d3d590b6d6b2921d09165b3da0432dbbe0`  
		Last Modified: Fri, 01 Oct 2021 03:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03687bcaf763a98e6c0f9a81d197c45dfd51dd2091cd530e78fbee30620fb340`  
		Last Modified: Wed, 13 Oct 2021 10:22:14 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4d0be3b18dc998fdb1808299e4103ca44fc43f048daf83393f1c78d705049b`  
		Last Modified: Wed, 13 Oct 2021 10:32:45 GMT  
		Size: 12.6 MB (12575791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65334ba197d55d794418a542b9bf8bf3e359010192ed5255ec921f03f0137dd`  
		Last Modified: Wed, 13 Oct 2021 10:32:45 GMT  
		Size: 208.6 KB (208556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:28b3a5a8502e5b4c517a64cb52c58c98d31ddd07252a1e7ef397fbbae08eaa56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102192911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270c9761f7c7e628d697a1c315a8b4be92cdab27f44702bbd4e62599fb12a579`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 05 Oct 2021 11:07:55 GMT
ADD file:361bb9cf514e8495ad6852f102582c401c790933bf4c44f858eeb9ac564def16 in / 
# Tue, 05 Oct 2021 11:08:00 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 12:58:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 05 Oct 2021 12:59:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 13:01:40 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Tue, 05 Oct 2021 13:02:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Oct 2021 13:02:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Oct 2021 13:03:03 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 06 Oct 2021 14:57:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 06 Oct 2021 14:57:17 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Oct 2021 14:57:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 06 Oct 2021 14:57:25 GMT
WORKDIR /usr/local/tomcat
# Wed, 06 Oct 2021 14:57:27 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 06 Oct 2021 14:57:30 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 06 Oct 2021 14:57:35 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 06 Oct 2021 14:57:38 GMT
ENV TOMCAT_MAJOR=10
# Thu, 07 Oct 2021 08:46:08 GMT
ENV TOMCAT_VERSION=10.0.12
# Thu, 07 Oct 2021 08:46:14 GMT
ENV TOMCAT_SHA512=e084fc0cc243c0a9ac7de85ffd4b96d00b40b5493ed7ef276d91373fe8036bc953406cd3c48db6b5ae116f2af162fd1bfb13ecdddf5d64523fdd69a9463de8a3
# Thu, 07 Oct 2021 08:46:17 GMT
COPY dir:ef4d2d5dbfee561c1886b5e1b39c2aae8ba009985e4bd8e34d0026f602a1c203 in /usr/local/tomcat 
# Thu, 07 Oct 2021 08:46:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Oct 2021 08:47:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 07 Oct 2021 08:47:16 GMT
EXPOSE 8080
# Thu, 07 Oct 2021 08:47:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b9dff9847c4194072c728793574720028129f446ababa16785403b9835c873f3`  
		Last Modified: Tue, 05 Oct 2021 11:10:52 GMT  
		Size: 33.3 MB (33290710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d0f93d81b8713c3abad0c3080f3bf43c08c0392ff1e24e640afa4e8a5ab59a`  
		Last Modified: Tue, 05 Oct 2021 13:08:20 GMT  
		Size: 17.2 MB (17207545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313973934c788499c2722d93b7d4bc276064db19094866558181f4b416cb590`  
		Last Modified: Tue, 05 Oct 2021 13:09:53 GMT  
		Size: 38.6 MB (38623829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c170bab519d9d468ce01a3712cf88d22e52ba968e7560cbd9a3d7a0c688e99`  
		Last Modified: Tue, 05 Oct 2021 13:09:45 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fa2bf0038fcb16cc68d2041f78f80bbb6ec8ad308e553f0eaf0b304a2ac713`  
		Last Modified: Wed, 06 Oct 2021 16:49:09 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28276f803e19cd4afe8acade92f34918aa7f33bf81f4f2ffc2ba24724cc886a2`  
		Last Modified: Thu, 07 Oct 2021 09:22:45 GMT  
		Size: 12.6 MB (12598879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772fdd7009296d44fc93950b0a1cd0d10d26d77d5c929337964726073223ce9`  
		Last Modified: Thu, 07 Oct 2021 09:22:43 GMT  
		Size: 471.5 KB (471484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3383dc857fb28559f72e16e46a0cd1e6ba708cf2af96eb70027d418668f116a3`  
		Last Modified: Thu, 07 Oct 2021 09:22:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:aede6885a6d88daea80f6abce8a2329361bf5aa9b4ef773a18eec50847273df3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93446064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:838f769e80867c0c88487281c95818b5799fba1fb553f94215a28cdde8696a3d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 00:58:54 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Sat, 16 Oct 2021 00:59:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 16 Oct 2021 00:59:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 00:59:18 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sat, 16 Oct 2021 01:33:54 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 16 Oct 2021 01:33:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 01:33:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 16 Oct 2021 01:33:55 GMT
WORKDIR /usr/local/tomcat
# Sat, 16 Oct 2021 01:33:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 16 Oct 2021 01:33:55 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 16 Oct 2021 01:33:55 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Sat, 16 Oct 2021 01:33:55 GMT
ENV TOMCAT_MAJOR=10
# Sat, 16 Oct 2021 01:35:57 GMT
ENV TOMCAT_VERSION=10.0.12
# Sat, 16 Oct 2021 01:35:57 GMT
ENV TOMCAT_SHA512=e084fc0cc243c0a9ac7de85ffd4b96d00b40b5493ed7ef276d91373fe8036bc953406cd3c48db6b5ae116f2af162fd1bfb13ecdddf5d64523fdd69a9463de8a3
# Sat, 16 Oct 2021 01:35:57 GMT
COPY dir:5e368530af9db760b4bb0e2613b782be098631a0d9cf6ca14736f1ab3721f2c3 in /usr/local/tomcat 
# Sat, 16 Oct 2021 01:36:01 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:36:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 16 Oct 2021 01:36:02 GMT
EXPOSE 8080
# Sat, 16 Oct 2021 01:36:02 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d87b2e49b2e5c452657363b2b41e85589fce56f6fd316b0ed01f396ff41282e`  
		Last Modified: Sat, 16 Oct 2021 01:01:25 GMT  
		Size: 37.6 MB (37564520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5814b6c6d297d74067c617cd3828d957d35648edcfb5ee6d5985748a01f1713`  
		Last Modified: Sat, 16 Oct 2021 01:01:21 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971ce99f351b1c125f6ab87dd8e0879116d05ca11e309a0d478c2db4452bbd2d`  
		Last Modified: Sat, 16 Oct 2021 01:45:13 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17e876d7ee92193345f7f88e8a41f324a88f7788d1c1f9be4697ec7c5f20a9`  
		Last Modified: Sat, 16 Oct 2021 01:46:22 GMT  
		Size: 12.6 MB (12571384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b17e6f929937d99d3e2306b5c269672ef97110d9ea03f4137cd1ecd2a033ef`  
		Last Modified: Sat, 16 Oct 2021 01:46:21 GMT  
		Size: 446.8 KB (446759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2ffb112c830908c1be283184f7f2874085e8f939e672c09f64740931d5a57e`  
		Last Modified: Sat, 16 Oct 2021 01:46:21 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
