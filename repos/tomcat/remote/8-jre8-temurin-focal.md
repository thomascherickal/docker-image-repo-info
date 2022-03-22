## `tomcat:8-jre8-temurin-focal`

```console
$ docker pull tomcat@sha256:57e239aaf95ab653cf71d076de4e7a863ed89a6a5134f60b23ba9ce6a569dfef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:8-jre8-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:8f472ec5d8bc0c87fb3b43dc2d78350d5eb5448eefa4f04dfc2b63e401f53592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98041656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19e8c899b5db7e60d3970a63700e8b634339d9b11cd9fb342f59fd2619a81e5e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:40 GMT
ADD file:1d3b09cf9e041d608a00c2dc25cdf3c388e436c5db607a3d124f2aa0f764fc69 in / 
# Fri, 18 Mar 2022 05:30:40 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 01:15:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 01:16:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 01:16:23 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 19 Mar 2022 01:16:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 19 Mar 2022 01:16:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 01:16:56 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sun, 20 Mar 2022 11:28:53 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sun, 20 Mar 2022 11:28:53 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 11:28:54 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sun, 20 Mar 2022 11:28:54 GMT
WORKDIR /usr/local/tomcat
# Sun, 20 Mar 2022 11:28:54 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 11:28:54 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 11:56:43 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sun, 20 Mar 2022 11:56:43 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Mar 2022 02:00:21 GMT
ENV TOMCAT_VERSION=8.5.77
# Tue, 22 Mar 2022 02:00:21 GMT
ENV TOMCAT_SHA512=50f96584cbbbeeda92a3b573e7fe7e2c49e57ed4bc5246257dc1409abac0710b49fa7049a0dd9a3b8467bca2aa078ef608f49b676c1abf12529528ff71bb0260
# Tue, 22 Mar 2022 02:00:22 GMT
COPY dir:ba423e7d738743f385aded444b8e3bfec67f9ef4472ff1e0a7456b085b195272 in /usr/local/tomcat 
# Tue, 22 Mar 2022 02:00:26 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Mar 2022 02:00:28 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Mar 2022 02:00:28 GMT
EXPOSE 8080
# Tue, 22 Mar 2022 02:00:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4d32b49e2995210e8937f0898327f196d3fcc52486f0be920e8b2d65f150a7ab`  
		Last Modified: Thu, 17 Mar 2022 11:55:39 GMT  
		Size: 28.6 MB (28565909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bca86330b80add24b2c91216395ff9d2a2e815b00c22f770434df27fef5335`  
		Last Modified: Sat, 19 Mar 2022 01:22:07 GMT  
		Size: 16.0 MB (16031105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303ed55001e972929edbe84ae3012f5755d614b7a65cab51a003bfe045d1e5d3`  
		Last Modified: Sat, 19 Mar 2022 01:22:38 GMT  
		Size: 41.8 MB (41773814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3008eb85a786ec8f914bbb926e4560cba97e99e595acea28b206245ff8644be`  
		Last Modified: Sat, 19 Mar 2022 01:22:31 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698338dfa3c11be475395ad3665960abcf5477b5f3613dd6127a1d7a37e00404`  
		Last Modified: Sun, 20 Mar 2022 12:18:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb361dfd47c6a7cbc090925347ee95ece7cc2dbb1b0068c4fd7c3127e9c443b`  
		Last Modified: Tue, 22 Mar 2022 02:21:43 GMT  
		Size: 11.2 MB (11225229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4807b316e83803d28a362dd8ff4dbaf32234e828463b8809620c297893eb79`  
		Last Modified: Tue, 22 Mar 2022 02:21:42 GMT  
		Size: 445.1 KB (445138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755cec8691f0ffaa548d29c440b80ffe1c7a12f61f439a679bfebceb8c212677`  
		Last Modified: Tue, 22 Mar 2022 02:21:42 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:d780c2e037c2e361779c145f65194befd5de508974a486b75e6b2c192474323f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90084559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88b1afff7e1c000473fe09b919866dc80894c36e410ae36a86899fffc22b7d43`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:32:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Mar 2022 06:33:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:33:29 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sun, 20 Mar 2022 06:34:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sun, 20 Mar 2022 06:34:27 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 06:34:28 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sun, 20 Mar 2022 21:04:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sun, 20 Mar 2022 21:04:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 21:04:39 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sun, 20 Mar 2022 21:04:39 GMT
WORKDIR /usr/local/tomcat
# Sun, 20 Mar 2022 21:04:40 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 21:04:40 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 21:22:07 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sun, 20 Mar 2022 21:22:07 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Mar 2022 01:54:53 GMT
ENV TOMCAT_VERSION=8.5.77
# Tue, 22 Mar 2022 01:54:54 GMT
ENV TOMCAT_SHA512=50f96584cbbbeeda92a3b573e7fe7e2c49e57ed4bc5246257dc1409abac0710b49fa7049a0dd9a3b8467bca2aa078ef608f49b676c1abf12529528ff71bb0260
# Tue, 22 Mar 2022 01:54:56 GMT
COPY dir:9ed3eb552accd9f76a54ed165181aca5f7da9b4ea19c8cb653c79a8d0328f39d in /usr/local/tomcat 
# Tue, 22 Mar 2022 01:55:06 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Mar 2022 01:55:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Mar 2022 01:55:09 GMT
EXPOSE 8080
# Tue, 22 Mar 2022 01:55:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53338e80157a2d8d75acf73c7d6a401a71fb6f4b5d452c1922a2452a516efef`  
		Last Modified: Sun, 20 Mar 2022 06:40:48 GMT  
		Size: 14.9 MB (14902387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880dc1148f62ba58fc19278629905a04a8bc619aed0ade19036c7b698a40fa55`  
		Last Modified: Sun, 20 Mar 2022 06:41:57 GMT  
		Size: 39.5 MB (39507633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cc11f5e063d6562262071ac7ea58f7b5bcf836363b4b4ebd14a17aa4e1c4d4`  
		Last Modified: Sun, 20 Mar 2022 06:41:36 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb368c7053e0ee708dc2b0cc9a7125ce62df1f239a723c1ecb919fe7184c7481`  
		Last Modified: Sun, 20 Mar 2022 21:40:55 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec9f3b6ebb3919aa05070a185ac8f0f97386eb0d669469cf21a59389df3693f`  
		Last Modified: Tue, 22 Mar 2022 02:12:58 GMT  
		Size: 11.2 MB (11177771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57034a5eda81c3e6c0e2cf6d769cf5f01824060269840ca8a2ee13792592023d`  
		Last Modified: Tue, 22 Mar 2022 02:12:54 GMT  
		Size: 422.8 KB (422821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898eb5f3cb08c351cc24ec201cb1cb2ed0452e5a317ab80ff5922b347972c1fc`  
		Last Modified: Tue, 22 Mar 2022 02:12:53 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:8682669dcd2683b3ee547186f733724812c74d8cc8486c7055bbb0e206a5be9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95289052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65587005871003f5ed9d84a8f28f374a2bd59ddd0a047819ce47760b7519f06`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:28:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 15:28:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:28:31 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 19 Mar 2022 15:28:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 19 Mar 2022 15:28:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 15:28:58 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 19 Mar 2022 23:02:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 19 Mar 2022 23:02:17 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 23:02:18 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 19 Mar 2022 23:02:19 GMT
WORKDIR /usr/local/tomcat
# Sat, 19 Mar 2022 23:02:20 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 19 Mar 2022 23:02:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 19 Mar 2022 23:33:41 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 19 Mar 2022 23:33:41 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Mar 2022 10:49:45 GMT
ENV TOMCAT_VERSION=8.5.77
# Tue, 22 Mar 2022 10:49:46 GMT
ENV TOMCAT_SHA512=50f96584cbbbeeda92a3b573e7fe7e2c49e57ed4bc5246257dc1409abac0710b49fa7049a0dd9a3b8467bca2aa078ef608f49b676c1abf12529528ff71bb0260
# Tue, 22 Mar 2022 10:49:48 GMT
COPY dir:ad610249dd56b12ec5099f9fed8207d79e1e99b4a4c75889504f93441a3af314 in /usr/local/tomcat 
# Tue, 22 Mar 2022 10:49:54 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Mar 2022 10:49:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Mar 2022 10:49:57 GMT
EXPOSE 8080
# Tue, 22 Mar 2022 10:49:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236902da3463f4b33e5af2f3ff655994cbe47d5e8380294ee6d6a5957b77710`  
		Last Modified: Sat, 19 Mar 2022 15:32:57 GMT  
		Size: 15.9 MB (15897447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578186aa0f8825663bbc5464445893d8e4b5d9c149e1e123555d5258c0b49904`  
		Last Modified: Sat, 19 Mar 2022 15:33:33 GMT  
		Size: 40.8 MB (40769840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe8e8c0b2e6d13d24d0d0afa7484a86287c8e9c4fb651eec691156959810857`  
		Last Modified: Sat, 19 Mar 2022 15:33:28 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd250619351da97822e84c0d6cacefd6c7ce4790dbf17c78124333db9d1187d`  
		Last Modified: Sun, 20 Mar 2022 00:00:06 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a2ffc2ee112557e0d0335cebcecbdaee2e239d5d5dc7ed6e56a31f6cc6568e`  
		Last Modified: Tue, 22 Mar 2022 11:23:44 GMT  
		Size: 11.2 MB (11243140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd331af743de7069ca9837060fa2d54ccb339d0492e208891397a433f9f575d`  
		Last Modified: Tue, 22 Mar 2022 11:23:43 GMT  
		Size: 208.7 KB (208742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:2ec9a35dd2190840ad49d6692f9bb644408076c61eba978b2dc7d703020177e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.4 MB (103397468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a025a797911e640040b8513a9439abd7f81d9720ece7cc6980dc4e1db7b7de58`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Mar 2022 00:48:28 GMT
ADD file:4f85f0964cc66c6d7dd6a29e535eb2235ff8847d3c3aa3342c74cc53710ae499 in / 
# Fri, 18 Mar 2022 00:48:34 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:09:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 20:10:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:10:33 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 19 Mar 2022 20:11:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 19 Mar 2022 20:11:26 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 20:11:30 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sun, 20 Mar 2022 21:07:35 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sun, 20 Mar 2022 21:07:36 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 21:07:42 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sun, 20 Mar 2022 21:07:44 GMT
WORKDIR /usr/local/tomcat
# Sun, 20 Mar 2022 21:07:46 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 21:07:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 21:42:00 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sun, 20 Mar 2022 21:42:01 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Mar 2022 02:35:56 GMT
ENV TOMCAT_VERSION=8.5.77
# Tue, 22 Mar 2022 02:36:03 GMT
ENV TOMCAT_SHA512=50f96584cbbbeeda92a3b573e7fe7e2c49e57ed4bc5246257dc1409abac0710b49fa7049a0dd9a3b8467bca2aa078ef608f49b676c1abf12529528ff71bb0260
# Tue, 22 Mar 2022 02:36:06 GMT
COPY dir:576971e7b168753cdfe4212aae8f5a1d95d6cc20fa0d0061b167653b570cc8bf in /usr/local/tomcat 
# Tue, 22 Mar 2022 02:36:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Mar 2022 02:37:01 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Mar 2022 02:37:02 GMT
EXPOSE 8080
# Tue, 22 Mar 2022 02:37:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cf1115d7b3bb72f50de3eb695005fb2c88fb88d73f535f164b306c4ab972c570`  
		Last Modified: Fri, 18 Mar 2022 00:51:19 GMT  
		Size: 33.3 MB (33292416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81c83f5d2456f061b5e8436215d94c771940ee113ed327dd33b701564ffa58e`  
		Last Modified: Sat, 19 Mar 2022 20:18:16 GMT  
		Size: 17.2 MB (17205279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e79e12f00cc2f2ad6a2f2a94bceb7063937e945931ff8fbda9c055408e37da4`  
		Last Modified: Sat, 19 Mar 2022 20:18:49 GMT  
		Size: 41.2 MB (41162315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bd6b17f427e5b43109e77cde332787886f2d266caff26f56cb4deba881c2ac`  
		Last Modified: Sat, 19 Mar 2022 20:18:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7dd5db736ccdf0772f77337771cfcbc5313570d5dc0910d2978ee30ba0e6e`  
		Last Modified: Sun, 20 Mar 2022 21:54:36 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523b3da26e99af3e184735faf3a2cfadae46fd32475f07193d7b9247e1dde88d`  
		Last Modified: Tue, 22 Mar 2022 02:47:12 GMT  
		Size: 11.3 MB (11265811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e918ead54c2b2f56c6cfca4f7ce2d2c18cde843354bcb1ee7aef1e4ec23e1`  
		Last Modified: Tue, 22 Mar 2022 02:47:11 GMT  
		Size: 471.2 KB (471181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241f098bf79e76d020341a3ecda4b29858655dabd2cf9162bce069f1d03ee0ab`  
		Last Modified: Tue, 22 Mar 2022 02:47:11 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
