## `tomcat:9-jre17-temurin`

```console
$ docker pull tomcat@sha256:8b8a95159d972160a9d3f7a467b8c3ffe0ff2e4f3912dcc3416ef515cb6ea7f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:9-jre17-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:9ecf53915491e20e15eb574e461c39e0ab022aeda67786ebbdc618c84d8a9b45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (107025202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fd3010cf7fbfff232b65774ed349acc745f103ca9ede16317735210d391d9a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:43:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:43:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:43:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:45:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:21:11 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:22:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:22:08 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:46:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:46:46 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:46:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:46:47 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:46:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:46:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:49:45 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 07 Nov 2022 21:49:45 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:04:03 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:04:03 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:04:03 GMT
COPY dir:4b420785e8457203dace88f2c45c4bf7ef041712c0106477a90d41f436650fa5 in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:04:07 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:04:08 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:04:09 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:04:09 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014fa72e018dd1c616d4bdb23d6fbb735820db9a943b470a787973556d4ee24e`  
		Last Modified: Wed, 02 Nov 2022 18:50:22 GMT  
		Size: 17.0 MB (16986189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27b0ce1a13407fdff72fe8b07ae4bd0b99dd436593bbc3510d89b2b3ff19c7f`  
		Last Modified: Mon, 07 Nov 2022 20:26:59 GMT  
		Size: 47.0 MB (46956964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23104d187cac450fd09c47d15ded1824ffe0432d1c58c97175d9970765b6000`  
		Last Modified: Mon, 07 Nov 2022 20:26:52 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1877470c5138c53a0b29a71d307ea45e2f694499535522f1c83e9e2259ea9202`  
		Last Modified: Mon, 07 Nov 2022 21:58:18 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd58b3a63bffc61b8182d74973bcf8422b06fb4d5e87c6d96c88ef645dcbe25b`  
		Last Modified: Tue, 15 Nov 2022 03:18:27 GMT  
		Size: 12.2 MB (12200283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49426ad4aefaeac6f370d74f4efe6d2dcb9d7eec4e6db0de46d051bef7634cf`  
		Last Modified: Tue, 15 Nov 2022 03:18:26 GMT  
		Size: 455.7 KB (455695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167b59e5447549124c2b0a86c46fa628b1613ef61241b3804ec5138f282eb534`  
		Last Modified: Tue, 15 Nov 2022 03:18:26 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:fbd503883dd4b42888a60543af86f7d54a2d30f4b10f45299179e96469d5106c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101192557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4cf227ef0959e6058af3e58938e7a7fb65e4b8cb1c78a201b1a07ec38d3160f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 17:58:54 GMT
ADD file:3acaa98e676fc52121edd2feea0fc71a60614dbf081f3db61809aab25af42a8c in / 
# Wed, 02 Nov 2022 17:58:54 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:35:35 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:35:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:35:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:39:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 19:59:00 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 19:59:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 19:59:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 20:44:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 20:44:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 20:44:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 20:44:38 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 20:44:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 20:44:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 20:49:07 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 07 Nov 2022 20:49:07 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 02:54:47 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 02:54:47 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 02:54:48 GMT
COPY dir:991468c955eccf0af966f6c16970656e9524632f0118e39a105322ae35e63d51 in /usr/local/tomcat 
# Tue, 15 Nov 2022 02:54:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:54:55 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 02:54:55 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 02:54:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3a947801223d5dd57236bed8663245ffddcbb4700ba3aec7edc7865fd8cd9d7`  
		Last Modified: Wed, 02 Nov 2022 18:00:26 GMT  
		Size: 27.0 MB (27020159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f20d187f670b7d0bfb9badfe46be4ee7a43d6bb8adb2e432aa10d941b76b3b`  
		Last Modified: Wed, 02 Nov 2022 18:48:39 GMT  
		Size: 17.1 MB (17107109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d03fb0da827c541aac3b10d93037131464e224ac7f48c31151bc0bec315224a`  
		Last Modified: Mon, 07 Nov 2022 20:04:46 GMT  
		Size: 44.5 MB (44500380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32fbc523239df88354e4423d6ec0ec13dfde1594130a226b400868c1d02ede1`  
		Last Modified: Mon, 07 Nov 2022 20:04:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d2bbd46c766df9790f1f61173fbb43e5b7f59063b6b5b5aaf8f692480dd440`  
		Last Modified: Mon, 07 Nov 2022 21:06:06 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86872c115e96f48ad15f1bd9ebb60f8a2daff98db6a28b8ff7ca649ca0b4a4cd`  
		Last Modified: Tue, 15 Nov 2022 03:17:59 GMT  
		Size: 12.1 MB (12135310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1c7a7c602bf09426d2039c358f6433400421512f864d56eccb0c3a611bf7c2`  
		Last Modified: Tue, 15 Nov 2022 03:17:59 GMT  
		Size: 429.2 KB (429171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de5908865fdee4d48e62cace0b6f7555f569c0141a0f0e147390b4969fea51`  
		Last Modified: Tue, 15 Nov 2022 03:17:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:e7a635afcbbab053403a4ca674c5905a8215bd37b151f178e1cfcb2cc0ed7d10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105852370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9eff9acc87671b32411e7bc8401e750ddc117219324ec51d7f1ea4187f11861`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:44:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 19:44:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 19:44:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 19:45:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:40:25 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:41:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:41:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:53:32 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:53:32 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:53:33 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:53:33 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:53:33 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:53:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:56:08 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 07 Nov 2022 21:56:08 GMT
ENV TOMCAT_MAJOR=9
# Mon, 07 Nov 2022 21:56:08 GMT
ENV TOMCAT_VERSION=9.0.68
# Mon, 07 Nov 2022 21:56:08 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Mon, 07 Nov 2022 21:56:09 GMT
COPY dir:08073dc914ff57f3e41125e7d2485fccf24cdd85202ccbc29412f228f068689f in /usr/local/tomcat 
# Mon, 07 Nov 2022 21:56:12 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:56:13 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Nov 2022 21:56:13 GMT
EXPOSE 8080
# Mon, 07 Nov 2022 21:56:13 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8d9c230ad7b20621780183623ce76b7c296e1db90d16a51deeb03f19e2493c`  
		Last Modified: Wed, 02 Nov 2022 19:49:51 GMT  
		Size: 18.4 MB (18416178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc0fa18ca42367edd695297ee17e1051d58c26adc5a55c6fb59006c6e942ccd`  
		Last Modified: Mon, 07 Nov 2022 20:44:50 GMT  
		Size: 46.4 MB (46398592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2734191cf33336ec1d8bbe61fe990127b53e477a84e337f11b0df19ae7b9cc`  
		Last Modified: Mon, 07 Nov 2022 20:44:44 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42ee5c97cd2e76389f89bf01d295d9bd3c8ea7631efb26081411481a5fd92cc`  
		Last Modified: Mon, 07 Nov 2022 22:04:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78311cffb9445474d25dbdca95ee4eecefe8760146610f81325bac7491af60d9`  
		Last Modified: Mon, 07 Nov 2022 22:07:21 GMT  
		Size: 12.2 MB (12200390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92412b1d8a4d2b3df46cb0e74bc14251976cceffa89eb4aaea147ae519900abb`  
		Last Modified: Mon, 07 Nov 2022 22:07:21 GMT  
		Size: 454.6 KB (454595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5b90f6a4ecd8ce972ba3c7afb78283ac2adf33d195a85e5394702286bac4e5`  
		Last Modified: Mon, 07 Nov 2022 22:07:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:fe5046ef90d42c5ccbc69999b3843c5ce83d0313c4362a1bc14ab1334237c59f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113497853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1574036b80ca02883000fa3f3aafe7b84b0a8ba528497418274c5f83039fccff`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:55:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:55:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:58:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:18:26 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:19:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:19:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:05:56 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:05:57 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:05:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:05:59 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:05:59 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:06:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:12:04 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 07 Nov 2022 21:12:04 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:29:39 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:29:39 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:29:40 GMT
COPY dir:fd9529113ac928cea114b7c17a20009f11466897b46f24368dc5549b3a9a5140 in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:29:49 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:29:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:29:51 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:29:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fe2e370e5759a8234c141ecd75ab498566337bfc051b67092071074afa4660`  
		Last Modified: Wed, 02 Nov 2022 19:06:05 GMT  
		Size: 18.3 MB (18267711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15dbf805c8926bab3c3a3bd0c694367d96e3de88d1cfe5825def5aa8b1a65f2`  
		Last Modified: Mon, 07 Nov 2022 20:26:28 GMT  
		Size: 46.8 MB (46807541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da969c3dcd44488aecff0aa22545753c040ef651eef86798cae09147ea76da18`  
		Last Modified: Mon, 07 Nov 2022 20:26:16 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c4f88acbef6c8446dd5b2c8356910b77042301c040eb2c79714ac00123e360`  
		Last Modified: Mon, 07 Nov 2022 21:28:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13d92e0b3dce2b28e63eae5d28d0a1cae3ec4a4d7d7542f6f3d9239bb7ff441`  
		Last Modified: Tue, 15 Nov 2022 03:52:01 GMT  
		Size: 12.2 MB (12228043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb526d1cce149f95da73c149e7f93816361c7ac1d9ed094939ba885abc58da`  
		Last Modified: Tue, 15 Nov 2022 03:52:00 GMT  
		Size: 486.5 KB (486514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba954e3d18e9f5b5e9d877d48b1fbccd773fe70c0f3e6ec659a4cf5047ae5b0e`  
		Last Modified: Tue, 15 Nov 2022 03:51:59 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:c7ff171393281df5934dfc015652b6ab47cf91df1a2a87a0851d84f39144076e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101788833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e2468dc31fa1f4428a96086f3418598fa0cc8fdefa4ddfbcaea010b7716c2a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:16:19 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 19:16:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 19:16:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 19:18:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:43:31 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:45:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:45:28 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:31:28 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:31:29 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:31:30 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:31:31 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:31:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:31:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:38:50 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 07 Nov 2022 21:38:50 GMT
ENV TOMCAT_MAJOR=9
# Mon, 07 Nov 2022 21:38:51 GMT
ENV TOMCAT_VERSION=9.0.68
# Mon, 07 Nov 2022 21:38:52 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Mon, 07 Nov 2022 21:38:53 GMT
COPY dir:8d2b4638bf6513026992e9ff60eac7beb13f8cf4d780d036c3e41007cf07e21b in /usr/local/tomcat 
# Mon, 07 Nov 2022 21:39:02 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 21:39:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Nov 2022 21:39:06 GMT
EXPOSE 8080
# Mon, 07 Nov 2022 21:39:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02da0c9f2dec84ef0248aec86752fb0e9403db13689aa31f355080aa227a81f4`  
		Last Modified: Wed, 02 Nov 2022 19:24:01 GMT  
		Size: 16.8 MB (16763703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5def766a4fb514cdc1deafed4a3620e4fd4628172c1d6d8694e1d0f79fa6503`  
		Last Modified: Mon, 07 Nov 2022 20:49:26 GMT  
		Size: 43.7 MB (43736897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6935aa87b9dd663c32d6c64f94c0320e0609dc34fdcdcd708fd5a4fb308d304`  
		Last Modified: Mon, 07 Nov 2022 20:49:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566aacc539ecedce76189f558873e3b73d1622fef1d1319b6ea719bca5d05a8d`  
		Last Modified: Mon, 07 Nov 2022 21:54:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213787e18d5ae7b045fb795f6c72635591128f20cdedacdc48065b7f54ce36c0`  
		Last Modified: Mon, 07 Nov 2022 21:57:49 GMT  
		Size: 12.2 MB (12189920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e445f985b2e4d26498ebcd47af3c5e5ec32c8607fb779a638f390b9bd0fbb43`  
		Last Modified: Mon, 07 Nov 2022 21:57:48 GMT  
		Size: 457.1 KB (457095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88c80672aa0e49e7fadd1613ae43285802234c260c253e26804f5a9b5c45742`  
		Last Modified: Mon, 07 Nov 2022 21:57:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
