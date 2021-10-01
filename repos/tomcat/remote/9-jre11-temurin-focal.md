## `tomcat:9-jre11-temurin-focal`

```console
$ docker pull tomcat@sha256:b94ff636cb2edd6416b3e26ee1531f5641f166bb7c973198d8d2a9c472a2c17b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:9-jre11-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:ac66a4f66ac48d98ffc8a3c44aa9498d1d38d15bae3bade2148f0394a1185c88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100512332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df7875aa00cabf7665b6c72b18d5321298f48b05dccc2d0382ff9c983dcb546`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:26:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 03:31:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Sep 2021 23:20:01 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 22 Sep 2021 19:56:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 22 Sep 2021 19:56:40 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Sep 2021 19:56:41 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 22 Sep 2021 20:24:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Sep 2021 20:24:45 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Sep 2021 20:24:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Sep 2021 20:24:46 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Sep 2021 20:24:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Sep 2021 20:24:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Sep 2021 20:29:47 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 22 Sep 2021 20:29:47 GMT
ENV TOMCAT_MAJOR=9
# Wed, 22 Sep 2021 20:29:47 GMT
ENV TOMCAT_VERSION=9.0.53
# Wed, 22 Sep 2021 20:29:47 GMT
ENV TOMCAT_SHA512=ee731b2d0c3ab7e14fa924dcb8d598707cedf714c9ce1f2c2d907a1fd51e26f7eec1343c3dc39e240ff64dac2e0213f154d23e5f94a430f429165b5df51f786f
# Wed, 22 Sep 2021 20:29:48 GMT
COPY dir:f0db5b070a8305c6b6d2c057f2bf6385d3a5ba472176591e87fed1c2b49631a3 in /usr/local/tomcat 
# Wed, 22 Sep 2021 20:29:52 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Sep 2021 20:29:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 22 Sep 2021 20:29:54 GMT
EXPOSE 8080
# Wed, 22 Sep 2021 20:29:54 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df1ad422e5a232e54d515fb2475eee78b57b25d905611bbceb50f364c0150c`  
		Last Modified: Tue, 31 Aug 2021 03:33:27 GMT  
		Size: 16.0 MB (16032853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9180a8ad3c00978420b5422374c9bc9f6aebd9f2d3def05292cc6dfe9e97bc51`  
		Last Modified: Wed, 22 Sep 2021 19:59:51 GMT  
		Size: 43.2 MB (43219898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73f5e84af8b081f0a260e3e9c669e083ee42425216b2b34bd378a3191e7d680`  
		Last Modified: Wed, 22 Sep 2021 19:59:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c935841a22c0c1ece8151abb61eeeffb3f086a311c2b1604cbde7b090c0f5a04`  
		Last Modified: Wed, 22 Sep 2021 20:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f7f30e61b0695e21895b5f6a82df022c04c8b17a178b879f7427ecd9ac8f4`  
		Last Modified: Wed, 22 Sep 2021 20:48:16 GMT  
		Size: 12.2 MB (12243486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e0e3b3772103d144432f5bbdb98716e783f12fc70f523393f7c1f347eae9f7`  
		Last Modified: Wed, 22 Sep 2021 20:48:15 GMT  
		Size: 445.6 KB (445560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447a29ffd94bcbfd95227a2969439b3f92199f8269a32d3290381f1280d73a7`  
		Last Modified: Wed, 22 Sep 2021 20:48:14 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:d272f6d163cb07f3d67709da87329ff9fe29ff68d153c8bd9684a23cf9a0ad04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93417326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a2f95e2da7d1378930b65daf10681410c4c7dbc74536a48ffe85a5d41b1fab0`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:51:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 22 Sep 2021 20:40:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Sep 2021 20:40:48 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 22 Sep 2021 20:42:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 22 Sep 2021 20:42:03 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Sep 2021 20:42:04 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 01 Oct 2021 03:31:20 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Oct 2021 03:31:21 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 03:31:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Oct 2021 03:31:23 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Oct 2021 03:31:23 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 03:31:23 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 03:36:08 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 01 Oct 2021 03:36:08 GMT
ENV TOMCAT_MAJOR=9
# Fri, 01 Oct 2021 03:36:09 GMT
ENV TOMCAT_VERSION=9.0.53
# Fri, 01 Oct 2021 03:36:09 GMT
ENV TOMCAT_SHA512=ee731b2d0c3ab7e14fa924dcb8d598707cedf714c9ce1f2c2d907a1fd51e26f7eec1343c3dc39e240ff64dac2e0213f154d23e5f94a430f429165b5df51f786f
# Fri, 01 Oct 2021 03:36:11 GMT
COPY dir:2f875c1d35c6af4085ade755c1d1dc6e751e3d9f5fc985bcfd23b7e563371e28 in /usr/local/tomcat 
# Fri, 01 Oct 2021 03:36:21 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:36:25 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Oct 2021 03:36:25 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 03:36:25 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38ad2952682521263306c30b66265ca7508f3287f2cfd9b8cb935f2a0be95fd`  
		Last Modified: Wed, 22 Sep 2021 20:43:33 GMT  
		Size: 14.9 MB (14902107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2be2f5f4c436b91c0bd4eb14087f379c4b1d094375a3091790ce4f5feb8d0eb`  
		Last Modified: Wed, 22 Sep 2021 20:45:15 GMT  
		Size: 41.8 MB (41831584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581c09071229e7e7cf33792f3bb0674151c88381e733c268f8afe89a488df29a`  
		Last Modified: Wed, 22 Sep 2021 20:44:48 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddb703e7b44a386b4b87456ebeb281d117ee0130548cc003b89d2ab606aa4ee`  
		Last Modified: Fri, 01 Oct 2021 03:45:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991c4bc5b9f2bfe08d8824ef261d7150a97597badb462957bdb1de2bc6447eeb`  
		Last Modified: Fri, 01 Oct 2021 03:48:12 GMT  
		Size: 12.2 MB (12192225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a922dd83226b2f9dc418f1d251f2a4648895ded2f736c6c3e382bf24281b7cd3`  
		Last Modified: Fri, 01 Oct 2021 03:48:08 GMT  
		Size: 422.1 KB (422124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e889a26bfe8bb8bff2cfa56e1fefaffc70d4bf12ca9583a0d290066eee9fb019`  
		Last Modified: Fri, 01 Oct 2021 03:48:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:0e889f55289edae6579ff0125af6cec1b1f554bc4fecef8ffb1c6c46e0958263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.3 MB (97291663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c50bf3486137cab9a54257c57cf17a09ccbb2dcb3b9d7238c29e6ae9e18c8f9`
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
# Fri, 01 Oct 2021 06:30:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Oct 2021 06:30:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 06:30:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Oct 2021 06:30:27 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Oct 2021 06:30:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 06:30:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 06:42:15 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 01 Oct 2021 06:42:15 GMT
ENV TOMCAT_MAJOR=9
# Fri, 01 Oct 2021 06:42:16 GMT
ENV TOMCAT_VERSION=9.0.53
# Fri, 01 Oct 2021 06:42:16 GMT
ENV TOMCAT_SHA512=ee731b2d0c3ab7e14fa924dcb8d598707cedf714c9ce1f2c2d907a1fd51e26f7eec1343c3dc39e240ff64dac2e0213f154d23e5f94a430f429165b5df51f786f
# Fri, 01 Oct 2021 06:42:16 GMT
COPY dir:dd6096f2e6eb4f02fe769d62521a61272f1415f847f2bd718d7ab7f8e6dc8aee in /usr/local/tomcat 
# Fri, 01 Oct 2021 06:42:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:42:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Oct 2021 06:42:23 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 06:42:24 GMT
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
	-	`sha256:8327b77f45d819d7c2beb6b1cd3664b11e0637de552f507d3831c6a8ae2769f0`  
		Last Modified: Fri, 01 Oct 2021 07:17:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c85fa3edb984cba6cd54a8c990575b4a611d8e1e5abbedac3e22d7cd081a1eb`  
		Last Modified: Fri, 01 Oct 2021 07:26:11 GMT  
		Size: 12.3 MB (12258995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbdf2bfda2dba0dec81434964594cf95e8df04255d40125b08fe777b94420c2`  
		Last Modified: Fri, 01 Oct 2021 07:26:09 GMT  
		Size: 446.2 KB (446211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2dce445d8ac6ff72ca92ac3e3e6674d6840d6d2af4f28da4dff7a33bbe251b`  
		Last Modified: Fri, 01 Oct 2021 07:26:09 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:56582573d72b59cf7a350c2c33f999de8f0618a57b3a910e98f1d94adbbbdb1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101876447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01df38e5c3f4bcaafbdf48925e3f6f838ce69af1ac26fa6f49a655783b232ea7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:31:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 05:45:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 13 Sep 2021 20:42:15 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 22 Sep 2021 20:01:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 22 Sep 2021 20:01:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Sep 2021 20:01:59 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 22 Sep 2021 20:54:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Sep 2021 20:54:33 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Sep 2021 20:54:43 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Sep 2021 20:54:48 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Sep 2021 20:54:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Sep 2021 20:55:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Sep 2021 21:21:15 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 22 Sep 2021 21:21:19 GMT
ENV TOMCAT_MAJOR=9
# Wed, 22 Sep 2021 21:21:24 GMT
ENV TOMCAT_VERSION=9.0.53
# Wed, 22 Sep 2021 21:21:29 GMT
ENV TOMCAT_SHA512=ee731b2d0c3ab7e14fa924dcb8d598707cedf714c9ce1f2c2d907a1fd51e26f7eec1343c3dc39e240ff64dac2e0213f154d23e5f94a430f429165b5df51f786f
# Wed, 22 Sep 2021 21:21:39 GMT
COPY dir:884f7957c728d35b8667277cf72e9613cdb318211cd3e85866fb64c522d95f95 in /usr/local/tomcat 
# Wed, 22 Sep 2021 21:21:59 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Sep 2021 21:22:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 22 Sep 2021 21:22:16 GMT
EXPOSE 8080
# Wed, 22 Sep 2021 21:22:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22897a482fa0e59d16e7302ee8b24736e577f4a14e821586507f289c961d84c9`  
		Last Modified: Tue, 31 Aug 2021 05:51:33 GMT  
		Size: 17.2 MB (17207875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9500c934ae44f69f3054ae17aae8a3e26fc9777f0206e871b8f37eb3ba77d47`  
		Last Modified: Wed, 22 Sep 2021 20:08:28 GMT  
		Size: 38.6 MB (38623880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a7579bb91cd6330c936ffe74be84e0ffde7f37994d184335a0305eda7a9ef2`  
		Last Modified: Wed, 22 Sep 2021 20:08:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed100d26ff82218f301110403156ef6526ca4e88133569cf2c005277fa7a0c37`  
		Last Modified: Wed, 22 Sep 2021 21:57:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb99007599c1eb83b86a01f934e77695a15bd573b1aba0ce8ba240ddd5fb907e`  
		Last Modified: Wed, 22 Sep 2021 22:00:44 GMT  
		Size: 12.3 MB (12281111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b633dbce30b9381f64fbace1c88a63666fc05d82a1f43691192c92016636d980`  
		Last Modified: Wed, 22 Sep 2021 22:00:43 GMT  
		Size: 471.3 KB (471328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054173cd99dd4e52035ede30ee1adf5d5977882e883cd4e9896626a12fc209c9`  
		Last Modified: Wed, 22 Sep 2021 22:00:42 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:e86ff553a8619b2053ace50009e019a92beb68853cf7d34a9414876f543b1db5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93128203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b64d10fd68d50503b07ecbaef78719b182b462e7d6db1c331e27defcb869af1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:00:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 02:45:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:45:11 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Fri, 01 Oct 2021 02:45:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eebf9b6b515fd139d45410ea4a0e7c18f015acba41e677cd7a57d1fe7a553681';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='814533727192258f45466784fb78d635994ed7051b911688401d1493bba38e91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='21129821a148503333dcc9868f04f3c971290c75f07ca384b1ab5d906901ea80';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='17932e94e7daa84057e20f99536cc66ab5ff52637b50bd5c1dfdcc1853aad0a9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e813e270b7ea0a13f9c400ce5abd4cb811aacbd536b8909e6c7f0e346f78348c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 01 Oct 2021 02:45:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 02:45:35 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 01 Oct 2021 04:44:53 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Oct 2021 04:44:53 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 04:44:53 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Oct 2021 04:44:54 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Oct 2021 04:44:54 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 04:44:54 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Oct 2021 04:48:46 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 01 Oct 2021 04:48:46 GMT
ENV TOMCAT_MAJOR=9
# Fri, 01 Oct 2021 04:48:46 GMT
ENV TOMCAT_VERSION=9.0.53
# Fri, 01 Oct 2021 04:48:47 GMT
ENV TOMCAT_SHA512=ee731b2d0c3ab7e14fa924dcb8d598707cedf714c9ce1f2c2d907a1fd51e26f7eec1343c3dc39e240ff64dac2e0213f154d23e5f94a430f429165b5df51f786f
# Fri, 01 Oct 2021 04:48:47 GMT
COPY dir:d52bc124bc9f022e5c2d9f1c9c83daf524d82961a8ea12bc440b9c97aaab568b in /usr/local/tomcat 
# Fri, 01 Oct 2021 04:48:50 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:48:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Oct 2021 04:48:52 GMT
EXPOSE 8080
# Fri, 01 Oct 2021 04:48:52 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ea6869b37d6809b4bdfbfc83b247246d2b56380b1c1f285e93eeabdda12def`  
		Last Modified: Fri, 01 Oct 2021 02:47:18 GMT  
		Size: 15.7 MB (15739143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58703680b3acf9898929e7513bb9e07d1caf651d840f92276ff1aacd7952f9e0`  
		Last Modified: Fri, 01 Oct 2021 02:47:41 GMT  
		Size: 37.6 MB (37564537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36346b91893ae9e4f2bc332c8149368577d9d4781fb1dcadc1c2d323b08031`  
		Last Modified: Fri, 01 Oct 2021 02:47:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0c4cd8a38fef08b1fc0af0acca383d63b64abcb0a71dc06014c48918ba2b0a`  
		Last Modified: Fri, 01 Oct 2021 04:54:49 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76da2e41fdb0b81b35ba3fefa227803ac9e18cf828293c3909c03be1fdcef2d`  
		Last Modified: Fri, 01 Oct 2021 04:56:55 GMT  
		Size: 12.3 MB (12254364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5325bdb2198a666a62d4f359537838d91b659964fad03022d4a7eb038190cef`  
		Last Modified: Fri, 01 Oct 2021 04:56:54 GMT  
		Size: 446.8 KB (446788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4cb3c9f61c1f092972057b78cbba4af622a7dc50df44e737465e00220de128`  
		Last Modified: Fri, 01 Oct 2021 04:56:54 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
