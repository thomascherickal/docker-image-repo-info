## `tomcat:8-jre17-temurin-focal`

```console
$ docker pull tomcat@sha256:fdc342f599664d8ef347680d1b1d0402b9415c1b048d6117b256a3e8a9264338
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jre17-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:13c416a27f6852b9f2f701648d289400e7a2ec0c4bfa9920d98314f0caa24109
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107367557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab84cb72115d99494c8d67b61562a52f6d0ea9edae6eb5b6fdc6acce6785f685`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 01:42:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 01:42:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 01:45:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:45:22 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 01:46:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 01:46:26 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 07:46:12 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 07:46:12 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:46:13 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 07:46:13 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 07:46:13 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:46:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:55:43 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 07:55:43 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 03:06:37 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 03:06:37 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 03:06:38 GMT
COPY dir:94c72f21878281b870486cc5499fe88fbd0ae69b594ba411ab8e952c61291a71 in /usr/local/tomcat 
# Fri, 20 Jan 2023 03:06:42 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 03:06:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 03:06:44 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 03:06:44 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b0873b98ac8f32b151346adbb3bebb71422b7f4d491cef4fe8fa08d19bf076`  
		Last Modified: Fri, 09 Dec 2022 01:52:23 GMT  
		Size: 20.1 MB (20086897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a502e2cfaa51a64df04eae97cd6f2f2d99ca4fbcd4419f6bc9aed960e9882`  
		Last Modified: Fri, 09 Dec 2022 01:53:22 GMT  
		Size: 47.0 MB (46956274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459bdc265a8a62e4ecc0b7303d8268d09e98cab20931a8dec69443564d9f72db`  
		Last Modified: Fri, 09 Dec 2022 01:53:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0347a6db3dfa3b4b72b9d23fbf1b3e86dc03c69a0977dc2f55b42c06b755e0df`  
		Last Modified: Fri, 09 Dec 2022 08:08:33 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41a7c8f9328076f2c296ca865a4eea534425fe4e4a5375e0398b7f3adc891bf`  
		Last Modified: Fri, 20 Jan 2023 03:18:52 GMT  
		Size: 11.3 MB (11295378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead865cc182e5cc8c86d8f1aeb375287316629585d41454fe7a171bc62d69be6`  
		Last Modified: Fri, 20 Jan 2023 03:18:51 GMT  
		Size: 451.7 KB (451666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e8c5891215c8fa0466b05e5b5b113f1e3c9533e5567c36efd8e438aaa2168a`  
		Last Modified: Fri, 20 Jan 2023 03:18:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:61ed375bf54d2c7177db882d437e5c7ce09a269e9a7ecbe9f3a068f775640d24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.2 MB (100227270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cbd83c3d085248517861ccc71be5d5303979ff8e74016339f3b297771adec07`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:16 GMT
ADD file:b21aa237ba47147762a1b92947251163795189df45212a32e07ea3438a186e03 in / 
# Fri, 09 Dec 2022 01:36:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:07:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:07:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:07:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:10:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:10:50 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 03:12:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:12:19 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 04:50:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 04:50:47 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 04:50:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 04:50:47 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 04:50:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 04:50:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 05:02:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 05:02:17 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 02:15:25 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 02:15:26 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 02:15:26 GMT
COPY dir:33b78f874243d55a25b75b9a840ac55cc4b377fb4b7df8c83c6bf771934696c1 in /usr/local/tomcat 
# Fri, 20 Jan 2023 02:15:31 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 02:15:32 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 02:15:32 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 02:15:32 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cfbc8b467b3eb89e7c394402566b2965c83f3103dafb141203e0020a8acd3774`  
		Last Modified: Fri, 09 Dec 2022 01:38:40 GMT  
		Size: 24.6 MB (24589003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c28baf7ed12652cd7f4e26e1feed9e86c3f06e9e323f65f77388748b92781c`  
		Last Modified: Fri, 09 Dec 2022 03:20:19 GMT  
		Size: 19.5 MB (19464848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91474906434c7a76ff0b33ab8f5ec5032282f2467769af66cd68dddda1deb439`  
		Last Modified: Fri, 09 Dec 2022 03:21:29 GMT  
		Size: 44.5 MB (44500857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd126692ffe353110c6008765c265e189ce2fe08a2e56eeff8307b63847e188a`  
		Last Modified: Fri, 09 Dec 2022 03:21:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e20d3b62e401c2b6cb49b64935051fdf00d79ef5c7f6162e1dc8b3e59af27df`  
		Last Modified: Fri, 09 Dec 2022 05:26:13 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a7fadf2de7ca1f6e6933150d5f8629391a2fb7ba2693ae52f99bb757909704`  
		Last Modified: Fri, 20 Jan 2023 02:33:26 GMT  
		Size: 11.2 MB (11242904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b73feac55a211304c33c6b979ba27d92acb7f803fb47a548b12450931c05a8`  
		Last Modified: Fri, 20 Jan 2023 02:33:24 GMT  
		Size: 429.2 KB (429232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5f347baa5c61a678121feed3a9b714f7e234790e929b26174c33e3cc4968d8`  
		Last Modified: Fri, 20 Jan 2023 02:33:24 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:5070ef55ac223ff4af5c1bd5609bee5620acd8a6c672e50c0c175ee5dfba7552
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.2 MB (106153569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0647058d7884b5456a944807a794a849b4ce44d813730e674830152c9f9cae69`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:38:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:38:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:38:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:41:25 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:41:25 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 03:42:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:42:24 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 06:22:11 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 06:22:11 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:22:12 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 06:22:12 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 06:22:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 06:22:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 06:29:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 06:29:57 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 03:26:19 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 03:26:19 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 03:26:19 GMT
COPY dir:37c13a9cd8431d817c6aa59bc86128d003701a1d44351733b2792da7b7759e8d in /usr/local/tomcat 
# Fri, 20 Jan 2023 03:26:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 03:26:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 03:26:24 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 03:26:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e6255f1d9634acbb611b17bafa5b0ec522018281353d85d93ff022b2cb8d08`  
		Last Modified: Fri, 09 Dec 2022 03:47:43 GMT  
		Size: 20.8 MB (20800924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4842b9157e67c223ff52e2b83e26b56da496dbea6b46c4a119a83d6ffb43a395`  
		Last Modified: Fri, 09 Dec 2022 03:48:33 GMT  
		Size: 46.4 MB (46398703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9191c480152f838e668fbfc5e95c440cafa592f303f581ead9215e025a001938`  
		Last Modified: Fri, 09 Dec 2022 03:48:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1857f266848dd8554350b35cac89cc729e0c12e54f53d8781b84c22096a95c`  
		Last Modified: Fri, 09 Dec 2022 06:42:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd75307edbcc57c04e545c53ea4a276fd15d319a86ed0b5fa404a618d67859f7`  
		Last Modified: Fri, 20 Jan 2023 03:37:52 GMT  
		Size: 11.3 MB (11309396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e8ad566b7c4e1717bdd0503f54aa5776841f1bd1c185aa6555b11317203d1`  
		Last Modified: Fri, 20 Jan 2023 03:37:51 GMT  
		Size: 450.9 KB (450915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31552ad920e2c36eeb75f08f5194fdf1e8dd67a9f27e3ff4c2b61caa1b48775d`  
		Last Modified: Fri, 20 Jan 2023 03:37:51 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:9b58c877b5daf611607c5243fb8c9bcd297e17306904cca4fc6c0c57af69c430
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113977380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad976333604cc309c3fd810e8cd33f2ceb11720d4cf749ec4d271c2d9dac39f6`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:36 GMT
ADD file:ca32a106475146fa5bd0f3e4920ea64671b1054f57a1f33d4681fe170deda313 in / 
# Fri, 09 Dec 2022 01:27:37 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:38:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 02:38:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 02:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 02:44:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:44:10 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 02:46:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 02:46:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 07:01:24 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 07:01:25 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:01:26 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 07:01:26 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 07:01:27 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:01:27 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:20:50 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 07:20:51 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 03:07:39 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 03:07:40 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 03:07:41 GMT
COPY dir:bbf334977ed9110e8bbff1ba54bb45f2967b7041a8397dd987587221f18fbf7f in /usr/local/tomcat 
# Fri, 20 Jan 2023 03:07:50 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 03:07:53 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 03:07:54 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 03:07:54 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d198f08d15a240101119086908bf4c5035dc657d52bfe206ddeede273c6b84f3`  
		Last Modified: Fri, 09 Dec 2022 01:30:09 GMT  
		Size: 33.3 MB (33299473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab1a4382d1a389e1c47c6c872157649690433c49f575b7c4f6d972d3c3dee2b`  
		Last Modified: Fri, 09 Dec 2022 02:56:45 GMT  
		Size: 22.1 MB (22058308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e37dfc20c7b716ec76a67cc9562fe5c570c0427b7c35fe2b4a5a34eedf1f5d`  
		Last Modified: Fri, 09 Dec 2022 02:58:21 GMT  
		Size: 46.8 MB (46807779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b70daeda21e7acd16245586178a724193832701ca89805de6ddfa6c5e058a0`  
		Last Modified: Fri, 09 Dec 2022 02:58:09 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c7123b3892669f75114d8d19e61689d1897d165b503f61c026fe2cafd8fe8b`  
		Last Modified: Fri, 09 Dec 2022 07:44:26 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388d8bbab71c4aaa54f95041785890d6d717ec71f98d5080eb89ad27c113640`  
		Last Modified: Fri, 20 Jan 2023 03:25:39 GMT  
		Size: 11.3 MB (11334501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8081fdee2cce7df8dfce949ca7850e108c36fc2493d49342425ad57276a6e5ca`  
		Last Modified: Fri, 20 Jan 2023 03:25:38 GMT  
		Size: 476.9 KB (476858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d5eda21349eb83fbaab213bf2ac52c6211f3032f3245ca8b5ae3bd3e9a12a0`  
		Last Modified: Fri, 20 Jan 2023 03:25:38 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:c699bf703a50e04aed941945651cce80bd04d029bcc81176c429ee096102d686
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (102041606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659713e02b882e891115b5aa996f40233657e48d6ac40387d789f6f839f39b03`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:52:40 GMT
ADD file:3d26982d2188d52ed2423587d3d2597c1f8ff614c19408d892cadc91d3743deb in / 
# Fri, 09 Dec 2022 01:52:43 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:11:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 02:11:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 02:11:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 02:15:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:15:59 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 02:18:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 02:18:23 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 04:42:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 04:42:06 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 04:42:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 04:42:09 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 04:42:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 04:42:10 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 04:50:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 04:50:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 00:46:37 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 00:46:37 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 00:46:38 GMT
COPY dir:87fcbe3d684aa2e3fcae2fc39dcdaa7779a7a5db17c33b11c0a25606c50e891c in /usr/local/tomcat 
# Fri, 20 Jan 2023 00:46:45 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 00:46:47 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 00:46:47 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 00:46:47 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5d330d9ae4f68425a719ebb93a3911994ee56b1328cf256fc3c44a4050de22ec`  
		Last Modified: Fri, 09 Dec 2022 01:54:57 GMT  
		Size: 27.0 MB (27016083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d57ebcbddf1c3cd78b6b6496f2fea9dc9a32bcce47843ed876abc3a51294ce2`  
		Last Modified: Fri, 09 Dec 2022 02:25:04 GMT  
		Size: 19.5 MB (19527858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7220fb304b6bd7a55bd7d77ae0b73a2eaa863d173da6530805d4adfc7306546d`  
		Last Modified: Fri, 09 Dec 2022 02:25:54 GMT  
		Size: 43.7 MB (43737314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fa149eb8250221c7b363042e36bfa16c25e5e35ced548326a6ad3a78c4063f`  
		Last Modified: Fri, 09 Dec 2022 02:25:48 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b81cb47be2120be8ed76761d9204ab91d353f9e7a0b111b810ef38f770aaa4d`  
		Last Modified: Fri, 09 Dec 2022 05:04:15 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0821f66faf4df128c5c9fde3c324e7ee33d7320298e6b8c15fe93cff3c51ebdc`  
		Last Modified: Fri, 20 Jan 2023 00:56:44 GMT  
		Size: 11.3 MB (11306447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddfa95ef3a71d38137e60424436603a9258642cbbbadcaf6664a85cb492dca9`  
		Last Modified: Fri, 20 Jan 2023 00:56:44 GMT  
		Size: 453.4 KB (453441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4346e0482ecd5f4d092fdf72b33bedade7acc9dfa42e3820ded82d493299fa`  
		Last Modified: Fri, 20 Jan 2023 00:56:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
