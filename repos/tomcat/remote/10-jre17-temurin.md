## `tomcat:10-jre17-temurin`

```console
$ docker pull tomcat@sha256:304af3388428b19a08d6a98db03313a3f28a7c3bbb944c689865d4889b5bd12a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:10-jre17-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:aee084dd3bb546c1997d2205e5b1cdffae8abcadfb444d4b3d2170a709fc0e8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (107019124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f3e2f8b12ad602e021cdb9c5a4e0bd7469f69ea391335f9a4755838877428f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:01:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:01:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:01:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:04:12 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:04:12 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 02 Mar 2023 04:04:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:04:47 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 10:45:22 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 10:45:22 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:45:23 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 10:45:23 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 10:45:23 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:45:23 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:46:08 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 02 Mar 2023 10:46:08 GMT
ENV TOMCAT_MAJOR=10
# Thu, 02 Mar 2023 10:46:08 GMT
ENV TOMCAT_VERSION=10.1.6
# Thu, 02 Mar 2023 10:46:09 GMT
ENV TOMCAT_SHA512=dd4bb415c2057eb6eedac1c29add6cf1eb4dfbd6658e9b889a4872b88464ee91c9dbe61d9d4c18f3c6ac479331952de956c708464459cb03b4803a8e9c297fa0
# Thu, 02 Mar 2023 10:46:09 GMT
COPY dir:a857f580743ffada32c576c6d9d84948d07b50b51a8c7b3abd6504c8ed1481c0 in /usr/local/tomcat 
# Thu, 02 Mar 2023 10:46:13 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 10:46:14 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 10:46:14 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 10:46:14 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b1a92356537d7da60fe31ae822ddc345f01a1be49b099c3b7d2bd576ae3b49`  
		Last Modified: Thu, 02 Mar 2023 04:10:40 GMT  
		Size: 17.0 MB (16975272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e504afe67521c2c247b6281da2fd3855688339eee739d255a086542fc67bf1d6`  
		Last Modified: Thu, 02 Mar 2023 04:11:33 GMT  
		Size: 46.9 MB (46935537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c732984ccf01fa98bce820be5b3ec0f48a9a0d85d8b48d190af249202bb8049`  
		Last Modified: Thu, 02 Mar 2023 04:11:26 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae018c5b2eb1a91463803b9530a94cdb0c9257842d305b70123db83788e98bb`  
		Last Modified: Thu, 02 Mar 2023 11:01:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fab09f312d11fc1885b946250663ebd5a73c3978adbe742110d3690457233e`  
		Last Modified: Thu, 02 Mar 2023 11:02:42 GMT  
		Size: 12.2 MB (12220904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf7569e17088a9d7d1d56ec7c8bdb7df07bd8a9c8a32cc691394d8e99218e7d`  
		Last Modified: Thu, 02 Mar 2023 11:02:41 GMT  
		Size: 456.9 KB (456948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffff87e380db42f7a0456ae33870b91084577053bf9c48b160f82a5a2f229ae`  
		Last Modified: Thu, 02 Mar 2023 11:02:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:e663b91c3451c169c29b41acffa6dab8859a4c57f0baa74ff00aa693f213257c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101272519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84a3dddaf4502b35a2e8f1441d9f7f2b49dee20c9a7a09d11661e724a8037050`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 10:59:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 10:59:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:59:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 11:03:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:03:03 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 02 Mar 2023 11:03:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 11:03:38 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 12:57:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 12:57:17 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 12:57:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 12:57:17 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 12:57:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 12:57:18 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 12:58:04 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 02 Mar 2023 12:58:04 GMT
ENV TOMCAT_MAJOR=10
# Thu, 02 Mar 2023 12:58:04 GMT
ENV TOMCAT_VERSION=10.1.6
# Thu, 02 Mar 2023 12:58:04 GMT
ENV TOMCAT_SHA512=dd4bb415c2057eb6eedac1c29add6cf1eb4dfbd6658e9b889a4872b88464ee91c9dbe61d9d4c18f3c6ac479331952de956c708464459cb03b4803a8e9c297fa0
# Thu, 02 Mar 2023 12:58:05 GMT
COPY dir:f381daeb7ac66f61310cb5bacccb2689f0164bbb4bb8f576fd268aa6ed6301ff in /usr/local/tomcat 
# Thu, 02 Mar 2023 12:58:09 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 12:58:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 12:58:10 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 12:58:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff13f7c3d7d759b64b6866366ce41218f9f783f9e2bd3c1a8a7fc284eb89472c`  
		Last Modified: Thu, 02 Mar 2023 11:09:57 GMT  
		Size: 17.1 MB (17093267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a8efee0c9a917933aed51d16c09b54aeece159fdfe0fa052e815cefb854fe0`  
		Last Modified: Thu, 02 Mar 2023 11:10:48 GMT  
		Size: 44.5 MB (44528851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6ea00bdaa53b8a420011a2901b1fc1f548877cbef37e7489b7cae55ab52de7`  
		Last Modified: Thu, 02 Mar 2023 11:10:40 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0aad7387483efaf876856a5ab7d889c8b6ca344458a918453fc1ec54aa9cae`  
		Last Modified: Thu, 02 Mar 2023 13:18:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db7556cd61aa39b995498ade3e9d136301d61792a7e63ae53cad8a11c5cc7a`  
		Last Modified: Thu, 02 Mar 2023 13:19:43 GMT  
		Size: 12.2 MB (12195440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9ed8d4cc543984b29c9f83ce5960f03325e20cbbba177afcb881cdddf42599`  
		Last Modified: Thu, 02 Mar 2023 13:19:42 GMT  
		Size: 430.0 KB (430009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faaa287a80b6df1543925ce2d384a95de1dff15cd93cfd5ecf30f35b2095333`  
		Last Modified: Thu, 02 Mar 2023 13:19:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:22e3c7b746b7aee0cf1fbde1be64c618bc339421984b10a99d7387f110dda986
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105888548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69df01145f19caf44d9974628f42e5654e8635fc48599c05c51f1960f89e81e5`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:27:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:27:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:27:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:30:07 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:30:07 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 02 Mar 2023 04:30:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:30:38 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 07:43:08 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 07:43:08 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:43:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 07:43:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 07:43:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:43:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:43:44 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 02 Mar 2023 07:43:44 GMT
ENV TOMCAT_MAJOR=10
# Thu, 02 Mar 2023 07:43:44 GMT
ENV TOMCAT_VERSION=10.1.6
# Thu, 02 Mar 2023 07:43:44 GMT
ENV TOMCAT_SHA512=dd4bb415c2057eb6eedac1c29add6cf1eb4dfbd6658e9b889a4872b88464ee91c9dbe61d9d4c18f3c6ac479331952de956c708464459cb03b4803a8e9c297fa0
# Thu, 02 Mar 2023 07:43:45 GMT
COPY dir:016cd8b2c8eebe8a359b26000d07f10732892edc4cb9e45a322ff5c9fae66356 in /usr/local/tomcat 
# Thu, 02 Mar 2023 07:43:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:43:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 07:43:49 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 07:43:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1945ba051ec7346afb985859773f982338590d9610191eeedbc86ffe6824de`  
		Last Modified: Thu, 02 Mar 2023 04:35:45 GMT  
		Size: 18.4 MB (18401218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c56b3a56e5ca7682fecb45863448a3c9283b5212c3d0e49e17316c0cbbb020`  
		Last Modified: Thu, 02 Mar 2023 04:36:26 GMT  
		Size: 46.4 MB (46421379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8ffb11de06bbc06e46b47b4faf1aa365d5fa2451107b4f0550448ff293dabb`  
		Last Modified: Thu, 02 Mar 2023 04:36:21 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc0ab256f609a62d16f1cf132dd22e6127822afb4b250069c53b94720f1b8e6`  
		Last Modified: Thu, 02 Mar 2023 07:57:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61df9b79f02312951fc2cc2e07da42e5ba8ef0250355f4b03945a9aea9c76a81`  
		Last Modified: Thu, 02 Mar 2023 07:58:18 GMT  
		Size: 12.2 MB (12221459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cae6e43ee853a92ada4905c90f22f9394794881dec11d9c3ae43feaaf004a3`  
		Last Modified: Thu, 02 Mar 2023 07:58:18 GMT  
		Size: 456.1 KB (456110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e248b625f4b2050bf50fe68867706450d4fc80f17044aed802ec903ad7d7f5`  
		Last Modified: Thu, 02 Mar 2023 07:58:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:31d1e40d2a0acf95eddc542b4c238d7f36f0e5d8d5c21b78b7e02e86c8acb1b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113473106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65579ee63a1468e3db435f44649c14113fa3a1f7373b13f3a27286a9abe37b1e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:04:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:04:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:04:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:10:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:10:43 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 02 Mar 2023 04:12:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:12:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 06:31:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 06:31:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 06:31:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 06:31:17 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 06:31:18 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:31:18 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:33:55 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 02 Mar 2023 06:33:55 GMT
ENV TOMCAT_MAJOR=10
# Thu, 02 Mar 2023 06:33:57 GMT
ENV TOMCAT_VERSION=10.1.6
# Thu, 02 Mar 2023 06:33:57 GMT
ENV TOMCAT_SHA512=dd4bb415c2057eb6eedac1c29add6cf1eb4dfbd6658e9b889a4872b88464ee91c9dbe61d9d4c18f3c6ac479331952de956c708464459cb03b4803a8e9c297fa0
# Thu, 02 Mar 2023 06:33:59 GMT
COPY dir:0a70c6d9dd97e2929d67383703cbfdce4eac92fb9ad4db7d22201c3ff9bbe421 in /usr/local/tomcat 
# Thu, 02 Mar 2023 06:34:16 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 06:34:19 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 06:34:20 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 06:34:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6285377bd773c7b29d366adba27fcbd8df16cebdc3aa9aaa4bec6c3fdf6f91e5`  
		Last Modified: Thu, 02 Mar 2023 04:21:56 GMT  
		Size: 18.3 MB (18257678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f65ad9a7690fb5ed5e91ed728b5f141ef3d3b97678ebcef3970c50818dfd2bb`  
		Last Modified: Thu, 02 Mar 2023 04:23:07 GMT  
		Size: 46.8 MB (46780994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2fbb0d715aa698759ab490956accad6caf4c50cc36ae0be0a74ec99aae44e4`  
		Last Modified: Thu, 02 Mar 2023 04:22:54 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168602f6e3339a0cac138353dc726d45d61e5c22566d81f4d1ed578bf23f3f70`  
		Last Modified: Thu, 02 Mar 2023 07:19:55 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44287215950735db6e34ea336d76f39bfa2d316f195d567f05e4d190dd0a6443`  
		Last Modified: Thu, 02 Mar 2023 07:21:26 GMT  
		Size: 12.2 MB (12234161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c4c0725901464015321d7835843e25a6796b4b347b670641797c054ad37d68`  
		Last Modified: Thu, 02 Mar 2023 07:21:25 GMT  
		Size: 488.2 KB (488221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847e43ea96651d877d8568845268ea5abec71021b7db67bd3a0422bdd7fac6b3`  
		Last Modified: Thu, 02 Mar 2023 07:21:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:bee40bc936a14df21bd8db6bc47087274e9c288ff238a5f8aa661ae0eac52ad3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (104011380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aef5d45afdc090075701a76fb8729d9e43e3fd38258c27b99139107f2d223a3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:59:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 17:59:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:59:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 18:00:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:00:58 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 31 Jan 2023 18:01:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 18:01:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 31 Jan 2023 19:53:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 31 Jan 2023 19:53:52 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 19:53:53 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 31 Jan 2023 19:53:53 GMT
WORKDIR /usr/local/tomcat
# Tue, 31 Jan 2023 19:53:53 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 31 Jan 2023 19:53:53 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 25 Feb 2023 00:04:31 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Sat, 25 Feb 2023 00:04:31 GMT
ENV TOMCAT_MAJOR=10
# Sat, 25 Feb 2023 00:04:31 GMT
ENV TOMCAT_VERSION=10.1.6
# Sat, 25 Feb 2023 00:04:31 GMT
ENV TOMCAT_SHA512=dd4bb415c2057eb6eedac1c29add6cf1eb4dfbd6658e9b889a4872b88464ee91c9dbe61d9d4c18f3c6ac479331952de956c708464459cb03b4803a8e9c297fa0
# Sat, 25 Feb 2023 00:04:31 GMT
COPY dir:e2dc0127e86179af89a37657f417e9da4894353fd73e2dd0b7cdacd88e8e8650 in /usr/local/tomcat 
# Sat, 25 Feb 2023 00:04:36 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Feb 2023 00:04:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 25 Feb 2023 00:04:37 GMT
EXPOSE 8080
# Sat, 25 Feb 2023 00:04:37 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028897ef38647e3545f5404bcb21a993ff6d9f6d87aeabe064f00b3df6f0d4cf`  
		Last Modified: Tue, 31 Jan 2023 18:06:38 GMT  
		Size: 16.8 MB (16753131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f1985bb4da0e0839208f17d9e4d1f0751949d50e9215e3ecb5da495235f71`  
		Last Modified: Tue, 31 Jan 2023 18:07:19 GMT  
		Size: 43.7 MB (43738795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1324cfa76418bb8277efd267984571f663e34d9fca270a09518caf4dff438890`  
		Last Modified: Tue, 31 Jan 2023 18:07:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7217ba34d335637a0b77eb8df45e0078af454ab71058f1c18205ab56caa5eaeb`  
		Last Modified: Tue, 31 Jan 2023 20:08:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a76cdf757e285477eb27490002a64dfe6a5bdd183d7932e69f2a174ba0e9406`  
		Last Modified: Sat, 25 Feb 2023 00:18:59 GMT  
		Size: 12.2 MB (12224400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e631644ecc4e459e39bd84a98b0c46d99702394f9cd7bae91664b4399de678`  
		Last Modified: Sat, 25 Feb 2023 00:18:59 GMT  
		Size: 2.7 MB (2652666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42315a69ca9c93762526a059d406326fa45abeea11ddfe1193c7111bf84559a`  
		Last Modified: Sat, 25 Feb 2023 00:18:58 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
