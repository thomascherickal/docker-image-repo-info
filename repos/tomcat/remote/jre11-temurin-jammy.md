## `tomcat:jre11-temurin-jammy`

```console
$ docker pull tomcat@sha256:e5720a020c059f7ee36debfce245b8bb4c4e15e3d27890501f6c4435b54681b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre11-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:7baf8898c586d2ddf8a5d97bd65de2bf52830a1f5592e77e9410770e11b38a4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102905252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f95eee658549ab5add8e590968e77b1317d865c06fec6dd4bfee711efb5b865`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:11:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 05:11:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 05:11:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 05:12:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:12:35 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 05:13:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 05:13:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 05:13:05 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 05:13:05 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 09:34:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Oct 2023 09:34:57 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 09:34:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Oct 2023 09:34:58 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Oct 2023 09:34:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 09:34:58 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 09:34:58 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 03 Oct 2023 09:34:58 GMT
ENV TOMCAT_MAJOR=10
# Fri, 13 Oct 2023 00:17:52 GMT
ENV TOMCAT_VERSION=10.1.14
# Fri, 13 Oct 2023 00:17:52 GMT
ENV TOMCAT_SHA512=53b7e8cc001686fe3893e00420b469c2d99f0065ee00d9e77e0f4eebdf41b77e69a2e5f27ce2dae2248116f5a78824144d7724c8dda1442b0796152cf7b09081
# Fri, 13 Oct 2023 00:17:52 GMT
COPY dir:6649bc889a4d0385da649653069ddccb107a40f658ca211d79d894f1834e37de in /usr/local/tomcat 
# Fri, 13 Oct 2023 00:17:56 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:17:58 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 13 Oct 2023 00:17:58 GMT
EXPOSE 8080
# Fri, 13 Oct 2023 00:17:58 GMT
ENTRYPOINT []
# Fri, 13 Oct 2023 00:17:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:707e32e9fc569fee476af9e92ae3d1df8b8e6dca47f9cb31db9d2c922a6de952`  
		Last Modified: Mon, 25 Sep 2023 12:54:05 GMT  
		Size: 30.4 MB (30440869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320d7b4a8f0a0932d6c981aa21a5793fb50fc408278be946023a29cdbe81594b`  
		Last Modified: Tue, 03 Oct 2023 05:16:04 GMT  
		Size: 12.9 MB (12902712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf200910a7c76a7a1bc2dffea3814986e9b71e5eb5c14062980bc3223a580d6`  
		Last Modified: Tue, 03 Oct 2023 05:17:20 GMT  
		Size: 46.9 MB (46864453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fec8b45ba806f43fc98549edb5fa09c6ad1aaf966b2b82b9c77f85d884a248a`  
		Last Modified: Tue, 03 Oct 2023 05:17:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cca1cb7fb758eeb83334e854da3070eaa354d251e96aba83d6e5bceb2f2435`  
		Last Modified: Tue, 03 Oct 2023 05:17:13 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51be1f327749acdd25cf2fe0dec3bb9e3e2c3fcc18d5b88dad9a5568f822c2bb`  
		Last Modified: Tue, 03 Oct 2023 09:45:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed6d48b7864de36177489b33928313caf8d3b2286692ac670536c932a918537`  
		Last Modified: Fri, 13 Oct 2023 00:46:09 GMT  
		Size: 12.2 MB (12240326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b262c37f4a8959517ea758c7e7b2d9b023e06304123d74ff6f71f0e71c7468ae`  
		Last Modified: Fri, 13 Oct 2023 00:46:08 GMT  
		Size: 455.7 KB (455697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8839e47312c8a4614763eecee2f55d2dba8b72c79f2b1c8dda6e4fc1971760`  
		Last Modified: Fri, 13 Oct 2023 00:46:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:513bfe5fac32d69881a4bb65023ec09233b9086a84de33bb584bcbec23c11a1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97664448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5671c7eae6ad2ff322f180929106e1818e63bbc6739265adb256a9cc3f9fc25`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 25 Sep 2023 10:19:15 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:19:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:19:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:19:16 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:19:18 GMT
ADD file:0008d56422c09f73afbcd40ace46d311e36ba0d60eef05198ea3665172ba3433 in / 
# Mon, 25 Sep 2023 10:19:18 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:00:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:00:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:00:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:01:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:02:05 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 06:02:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 06:02:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 06:02:29 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 06:02:29 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 06:56:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Oct 2023 06:56:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:56:16 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Oct 2023 06:56:16 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Oct 2023 06:56:16 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 06:56:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 06:56:17 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 03 Oct 2023 06:56:17 GMT
ENV TOMCAT_MAJOR=10
# Fri, 13 Oct 2023 00:10:42 GMT
ENV TOMCAT_VERSION=10.1.14
# Fri, 13 Oct 2023 00:10:42 GMT
ENV TOMCAT_SHA512=53b7e8cc001686fe3893e00420b469c2d99f0065ee00d9e77e0f4eebdf41b77e69a2e5f27ce2dae2248116f5a78824144d7724c8dda1442b0796152cf7b09081
# Fri, 13 Oct 2023 00:10:43 GMT
COPY dir:6ca044a24fa04698a0316b6e8879f32d956b8f704c14372ebaea6dd18d18e2ec in /usr/local/tomcat 
# Fri, 13 Oct 2023 00:10:47 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:10:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 13 Oct 2023 00:10:49 GMT
EXPOSE 8080
# Fri, 13 Oct 2023 00:10:49 GMT
ENTRYPOINT []
# Fri, 13 Oct 2023 00:10:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7271b2c80df6c73d794550b50f57d78c6fd5b85da7934c6506c76ea706087280`  
		Last Modified: Tue, 26 Sep 2023 02:07:56 GMT  
		Size: 27.5 MB (27515498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda8dd86380daebf30969cb41ed0b268657958a7e1447d39fc3a2fc0d9c8c636`  
		Last Modified: Tue, 03 Oct 2023 06:03:57 GMT  
		Size: 12.5 MB (12491478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f496e54e741199b5cf52fb27d70d5e8b72cab406852a0a971af0fda8b7077`  
		Last Modified: Tue, 03 Oct 2023 06:05:03 GMT  
		Size: 45.0 MB (45012599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7f8cf124bd8e3b73376ff7a7f099bb0296ee827fb2a0effa3d680e6cf6bd42`  
		Last Modified: Tue, 03 Oct 2023 06:04:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3404aca9dcfb64a64d8574f380cb6e9c20dc67bc15bdf62b297eb673f3ee695`  
		Last Modified: Tue, 03 Oct 2023 06:04:55 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d25e01a80defe6e28f3d9c94e275f74b26f542917d577f08adc9d21b38fb4ca`  
		Last Modified: Tue, 03 Oct 2023 07:04:52 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0daefa00505818472d188a604e030c42592c8654881b58cf91363241b20c616d`  
		Last Modified: Fri, 13 Oct 2023 00:25:01 GMT  
		Size: 12.2 MB (12213839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b216451a7707fc03fe423834eefc64acd4d1c6f467915aadc38490ec27c2c7`  
		Last Modified: Fri, 13 Oct 2023 00:25:00 GMT  
		Size: 429.8 KB (429839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b746f235733a83d5f6598936ddb476e537d95a21dc13d950a76c5aaa60acd4b`  
		Last Modified: Fri, 13 Oct 2023 00:24:59 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:3f6f543c531819213898233db8f861630c58b212d1fd5df53025084c9f707eb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99124908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:035c000d7e9107e9a81e4496658540c2cac9cddc7efa7ac969e49983f0b03fb3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:06:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:06:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:06:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:07:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:07:36 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 06:07:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 06:07:59 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 06:07:59 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 06:07:59 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 07:49:53 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Oct 2023 07:49:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 07:49:54 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Oct 2023 07:49:54 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Oct 2023 07:49:54 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 07:49:54 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 07:49:54 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 03 Oct 2023 07:49:54 GMT
ENV TOMCAT_MAJOR=10
# Fri, 13 Oct 2023 00:15:43 GMT
ENV TOMCAT_VERSION=10.1.14
# Fri, 13 Oct 2023 00:15:43 GMT
ENV TOMCAT_SHA512=53b7e8cc001686fe3893e00420b469c2d99f0065ee00d9e77e0f4eebdf41b77e69a2e5f27ce2dae2248116f5a78824144d7724c8dda1442b0796152cf7b09081
# Fri, 13 Oct 2023 00:15:44 GMT
COPY dir:095162b05c9584a70c0b081449f23610056428c24804c67b6bb384373085e458 in /usr/local/tomcat 
# Fri, 13 Oct 2023 00:15:47 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:15:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 13 Oct 2023 00:15:49 GMT
EXPOSE 8080
# Fri, 13 Oct 2023 00:15:49 GMT
ENTRYPOINT []
# Fri, 13 Oct 2023 00:15:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6ea603f1df5e3d23206761eca19fba4cdf4e22d773256cb65b71b730aa5acced`  
		Last Modified: Mon, 25 Sep 2023 17:30:11 GMT  
		Size: 28.4 MB (28392073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db904450c39fc4ef39317a37a19b15df4a74bf6bb91100343e382470ce034d79`  
		Last Modified: Tue, 03 Oct 2023 06:10:10 GMT  
		Size: 12.8 MB (12843603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30912c039dbaa796a9a5ed542699bef3d9a28d45ef6fffa82c09a17c4052a8fb`  
		Last Modified: Tue, 03 Oct 2023 06:11:17 GMT  
		Size: 45.2 MB (45190639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc4baa5de8169875cf5865d296a609c50890a7399b643ee1c70d96c34858f22`  
		Last Modified: Tue, 03 Oct 2023 06:11:12 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ccb257c1839235e5d23765c7e3a1a38f9d8f26fcb582bf489b3092f6ba4f59`  
		Last Modified: Tue, 03 Oct 2023 06:11:12 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe014e40db5b2327ab56545990d7cccba870416075c416bbb42e125a013345c`  
		Last Modified: Tue, 03 Oct 2023 07:59:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee7802fada8b075a617e1660f33fea8f9df7cf842df8249775f049294246780`  
		Last Modified: Fri, 13 Oct 2023 00:41:04 GMT  
		Size: 12.2 MB (12241463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a3468cd647b09eab25e96752dff0c4057ada94e3aad3136276745e8c95f8cd`  
		Last Modified: Fri, 13 Oct 2023 00:41:03 GMT  
		Size: 455.9 KB (455936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d825f3c9e90fc0bd57796b39e7c308044e9661e7ffd5c9b7ce02d9e855830dd`  
		Last Modified: Fri, 13 Oct 2023 00:41:02 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:ddbba92ba17637cd911ab32e95bf219f9764bd059986405227c8449729da28ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104477073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2918489d67a9e574ebccdc64abc5f70431465589a539804605c8a0044db3130`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 25 Sep 2023 10:20:46 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:20:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:20:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:20:46 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:20:49 GMT
ADD file:4e52928c778d7e98d90ccfcaacd039ae1fdde494dfa310adbe229d7051c30918 in / 
# Mon, 25 Sep 2023 10:20:49 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:16:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 08:16:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 08:16:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 08:17:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:18:25 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 08:19:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 08:19:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 08:19:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 08:19:18 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 11:47:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Oct 2023 11:47:29 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 11:47:30 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Oct 2023 11:47:31 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Oct 2023 11:47:31 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 11:47:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 11:47:32 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 03 Oct 2023 11:47:33 GMT
ENV TOMCAT_MAJOR=10
# Tue, 03 Oct 2023 11:47:34 GMT
ENV TOMCAT_VERSION=10.1.13
# Tue, 03 Oct 2023 11:47:35 GMT
ENV TOMCAT_SHA512=406c0c367ac6ad95bb724ecc3a3c340ad7ded8c62287d657811eeec496eaaca1f5add52d2f46111da1426ae67090c543f6deccfeb5fdf4bdae32f9b39e773265
# Tue, 03 Oct 2023 11:47:37 GMT
COPY dir:907364ecf0676cf0a47de0f674197a73ff9734e686fe10f18ba3c3aee0afd824 in /usr/local/tomcat 
# Tue, 03 Oct 2023 11:47:51 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 11:47:55 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 03 Oct 2023 11:47:56 GMT
EXPOSE 8080
# Tue, 03 Oct 2023 11:47:56 GMT
ENTRYPOINT []
# Tue, 03 Oct 2023 11:47:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:8098558aeb0337452acaa8c74f02401dc8e9bc5a2c048e4c82c013b483a11f11`  
		Last Modified: Tue, 03 Oct 2023 07:57:52 GMT  
		Size: 35.7 MB (35702863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931c9c8af9e87407323da067bbf3a8b691add055bcd0d602e17cd36b4b0c4cee`  
		Last Modified: Tue, 03 Oct 2023 08:22:20 GMT  
		Size: 13.8 MB (13770245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daba77c58e0218761122afd06661efcb276de0262b805e438dc5735125516b7`  
		Last Modified: Tue, 03 Oct 2023 08:23:37 GMT  
		Size: 42.3 MB (42294947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b31cae2de56f31de6fee776ac6d41714dc8520ea9ec6e6546b6db1f3dcde95`  
		Last Modified: Tue, 03 Oct 2023 08:23:28 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cefd3f92291efaafd2a4af9d10be842ddc18f75d8f7b2cac8b5efb7db710c4`  
		Last Modified: Tue, 03 Oct 2023 08:23:28 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0898e5505e5ae72d92a58d0a6f474f95752e8026f82eb476951996d6475052ca`  
		Last Modified: Tue, 03 Oct 2023 12:10:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b873b4fe0b93a988dc6235325f0ae91189828de2ffb3614b00191d9cbf3a1`  
		Last Modified: Tue, 03 Oct 2023 12:10:43 GMT  
		Size: 12.2 MB (12220814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8a1362c2b7a51b06c89359defc1626d708ecbbad8df968936cdba3bc9a47ac`  
		Last Modified: Tue, 03 Oct 2023 12:10:42 GMT  
		Size: 487.0 KB (487010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f284bca2bf8311592eb14efaf3be8a45b3a9a218c4c6b649d22e5bcc63c662ce`  
		Last Modified: Tue, 03 Oct 2023 12:10:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:f7497a725fb542143fb0df57b6aabe7c961be3f4cc34448573bf3bdb33a8165f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94932223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7f3c9c7c2386471d977a5ef98061e7522420238a05a129d3b11104fd380d1b7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:08:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 09:08:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 09:08:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 09:08:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:08:55 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 09:09:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 09:09:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 09:09:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 09:09:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 11:58:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Oct 2023 11:58:31 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 11:58:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Oct 2023 11:58:32 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Oct 2023 11:58:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 11:58:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Oct 2023 11:58:32 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 03 Oct 2023 11:58:32 GMT
ENV TOMCAT_MAJOR=10
# Tue, 03 Oct 2023 11:58:33 GMT
ENV TOMCAT_VERSION=10.1.13
# Tue, 03 Oct 2023 11:58:33 GMT
ENV TOMCAT_SHA512=406c0c367ac6ad95bb724ecc3a3c340ad7ded8c62287d657811eeec496eaaca1f5add52d2f46111da1426ae67090c543f6deccfeb5fdf4bdae32f9b39e773265
# Tue, 03 Oct 2023 11:58:33 GMT
COPY dir:9386c6cf86dffa3ac71746ad923462554a9871726f149dc0af90329531a8c8d0 in /usr/local/tomcat 
# Tue, 03 Oct 2023 11:58:38 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 11:58:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 03 Oct 2023 11:58:40 GMT
EXPOSE 8080
# Tue, 03 Oct 2023 11:58:40 GMT
ENTRYPOINT []
# Tue, 03 Oct 2023 11:58:40 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6ebbc5199f54e5da3b34aa5983900a17cba52d2381529b95064414261c04f7`  
		Last Modified: Tue, 03 Oct 2023 09:12:09 GMT  
		Size: 13.0 MB (12981189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182515bc828e094c1db47c74ce85971f300fe58a1f93cfab97a1cc8d63dca0d3`  
		Last Modified: Tue, 03 Oct 2023 09:12:49 GMT  
		Size: 40.6 MB (40632039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad87f3293ad6d670f1f4118fe39901731d4f25a26c468fbe1450d4ba8989a78`  
		Last Modified: Tue, 03 Oct 2023 09:12:43 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f19c003d44db6924c597b1941f29c5a3136a9b45ccafd50d16412a8130019ca`  
		Last Modified: Tue, 03 Oct 2023 09:12:43 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c75dab469af791a924b6f17b419ce5aaa6df299432613318077c3d4d2b9ea0`  
		Last Modified: Tue, 03 Oct 2023 12:18:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f231c06c0ad8b9f9340e7bd39abf13076465393d97fd3dbb162a61464975a8`  
		Last Modified: Tue, 03 Oct 2023 12:18:47 GMT  
		Size: 12.2 MB (12208605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e89a0d99cfaa07668f5ad357f7e7cc55ccd1a4b2d183de6934f6be3d899611`  
		Last Modified: Tue, 03 Oct 2023 12:18:46 GMT  
		Size: 457.2 KB (457215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fb412e3ce3bd160895400047ae2b35c408c9fd342ad5b2668fa73775f1d96c`  
		Last Modified: Tue, 03 Oct 2023 12:18:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
