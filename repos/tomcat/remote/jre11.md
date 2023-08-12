## `tomcat:jre11`

```console
$ docker pull tomcat@sha256:e258904b39c8ee918f80b16bdd85331ec666250552ca04e227879ded73ef700b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre11` - linux; amd64

```console
$ docker pull tomcat@sha256:7bfa95155a6d7bb7dfd414ce1800c5dcf6684e75c61d1d25dac8d8c9b4d8b8cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102883939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a131cef79da2413c822dfbcb634fdc12823486dc0930882b6fdfef4f31217c4`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:33:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:33:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:33:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:21:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:22:14 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:22:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:22:53 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:22:53 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:22:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 21:19:42 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 21:19:42 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:19:43 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 21:19:43 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 21:19:43 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:19:43 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:19:43 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 08 Aug 2023 21:19:43 GMT
ENV TOMCAT_MAJOR=10
# Tue, 08 Aug 2023 21:19:43 GMT
ENV TOMCAT_VERSION=10.1.11
# Tue, 08 Aug 2023 21:19:43 GMT
ENV TOMCAT_SHA512=ad754aa695898cf8af5b64f4e29da7013fb39f808a90fa0e030228680a17c01b10bb0904762417ebac99b075947e4ea26f2f22f5da2aa4e399237468b76fa4fb
# Tue, 08 Aug 2023 21:19:44 GMT
COPY dir:c3f897e2e9044a5b4da6be54a9d10fa962a3f809b8e7dde0708b37faa049643d in /usr/local/tomcat 
# Tue, 08 Aug 2023 21:19:47 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:19:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 21:19:49 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:16:23 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:16:23 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1d9603a2223f0c0337b5489031adc59113c119d64dfce6852f6114f42f2f05`  
		Last Modified: Tue, 08 Aug 2023 19:27:08 GMT  
		Size: 12.9 MB (12902861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ec547f8ce2155ce58a25da4ddaaffb94bbba064f0491bbc9535447779218de`  
		Last Modified: Tue, 08 Aug 2023 19:30:50 GMT  
		Size: 46.9 MB (46864855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c96886bebf4fd42e9a6622257a11b02a6c388c2a8b5dda93d1087b4f6ee1fd`  
		Last Modified: Tue, 08 Aug 2023 19:30:44 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf16da19f8ed2a380e226c2910876175263f8b9faadec9dc54ce22afa3d1af2`  
		Last Modified: Tue, 08 Aug 2023 19:30:44 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61848075b315b207168c2fe1398dab9d0ec71c4fbb107cb79e1905a1f8a45f6`  
		Last Modified: Tue, 08 Aug 2023 21:33:54 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a836f69d09676b5caf818dbf0e1d7fbe3501672453d7b84eccc2d0e5927ad2`  
		Last Modified: Tue, 08 Aug 2023 21:33:56 GMT  
		Size: 12.2 MB (12228228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea13490dafee844a62d57325240b1a707fa950433cf6d0ab6daa1632b0a044`  
		Last Modified: Tue, 08 Aug 2023 21:33:55 GMT  
		Size: 455.6 KB (455639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b9fe015e1e822a90353d814a5c4228b3e8298385deec9d0270d138f411385f`  
		Last Modified: Tue, 08 Aug 2023 21:33:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:df688b4afd0e3f972d25b81fe547ad1a42bc6c7b55a83dd858c167662581dcd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97162105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b296d699dad4b01445681fdd3d49d29c89bc412e795bfbc702d7b72651a2f97`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:09:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:09:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:09:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 18:59:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:00:03 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:00:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:00:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:00:33 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:00:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 19:56:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 19:56:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 19:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 19:56:27 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 19:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 19:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 19:56:28 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 08 Aug 2023 19:56:28 GMT
ENV TOMCAT_MAJOR=10
# Tue, 08 Aug 2023 19:56:28 GMT
ENV TOMCAT_VERSION=10.1.11
# Tue, 08 Aug 2023 19:56:28 GMT
ENV TOMCAT_SHA512=ad754aa695898cf8af5b64f4e29da7013fb39f808a90fa0e030228680a17c01b10bb0904762417ebac99b075947e4ea26f2f22f5da2aa4e399237468b76fa4fb
# Tue, 08 Aug 2023 19:56:29 GMT
COPY dir:d646edcd7d693176f20d7d6b67291f664c4f98a8fc9ec0476e0a8f1e6fa04a32 in /usr/local/tomcat 
# Tue, 08 Aug 2023 19:56:33 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:56:35 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 19:56:35 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:25:29 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:25:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791f420277f117d4cbc9798bac0e3991df4d76dcb209a6289b5474d81f4c32d0`  
		Last Modified: Tue, 08 Aug 2023 19:02:56 GMT  
		Size: 12.5 MB (12491020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488129ff542f9219b30a6eeb605366757b9f8a1ded3e35478e46e293c8c0702d`  
		Last Modified: Tue, 08 Aug 2023 19:04:54 GMT  
		Size: 45.0 MB (45013047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9327b04613d69a7cfb1d735b350938d15b93139ebc371bca95df06821c0ff23`  
		Last Modified: Tue, 08 Aug 2023 19:04:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcf4e3ac40244e0a4c3d631e214005a21c6af63accecd7cd1b70cbd1eae57f8`  
		Last Modified: Tue, 08 Aug 2023 19:04:47 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7966203b4d51d7c30d8b666be073bf177511881157c202cd86c01fdc8b81e0ae`  
		Last Modified: Tue, 08 Aug 2023 20:10:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429c4c0d27f53a2935209d4d5837aba41ff45a4b728a4bd7d4ca147f8e5b1906`  
		Last Modified: Tue, 08 Aug 2023 20:10:24 GMT  
		Size: 12.2 MB (12201029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913e9fbd7ab627d16bdd80c0a02f92a7f9dae35b47d564962327d6dfb7348374`  
		Last Modified: Tue, 08 Aug 2023 20:10:23 GMT  
		Size: 428.9 KB (428920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab12b8b40582e5e56ebfedd5d646cc6e4c36a36eb40d0557c26bcba83e6aba`  
		Last Modified: Tue, 08 Aug 2023 20:10:23 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:d84e0b12ad7c2969430bd2d058eb6e58bfa08cef6853f89c45b053d9a6a06acd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6b3ac956dde93925fb6a28df1354eb27acf3ff1400bdead64c3d7fd6d0157c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:32:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 15:32:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 15:32:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:40:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:41:25 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:41:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:41:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:41:51 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:41:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 22:35:53 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 22:35:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:35:54 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 22:35:54 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 22:35:54 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 22:35:54 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 22:35:54 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 08 Aug 2023 22:35:54 GMT
ENV TOMCAT_MAJOR=10
# Tue, 08 Aug 2023 22:35:54 GMT
ENV TOMCAT_VERSION=10.1.11
# Tue, 08 Aug 2023 22:35:54 GMT
ENV TOMCAT_SHA512=ad754aa695898cf8af5b64f4e29da7013fb39f808a90fa0e030228680a17c01b10bb0904762417ebac99b075947e4ea26f2f22f5da2aa4e399237468b76fa4fb
# Tue, 08 Aug 2023 22:35:55 GMT
COPY dir:e8493a2bd828e497d3211236dcbffc0e853cae221243f608cd55a656695cc6de in /usr/local/tomcat 
# Tue, 08 Aug 2023 22:35:58 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 22:35:59 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 22:35:59 GMT
EXPOSE 8080
# Tue, 08 Aug 2023 22:35:59 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91712d801b234a271df55fd60b35e7d2918ce5ae0fb7ce56a8de0edb8151fd0e`  
		Last Modified: Tue, 08 Aug 2023 19:44:21 GMT  
		Size: 12.8 MB (12844180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aeb71c3e8ddfbdbcdf7f366fa14814e5ae4bc3c34c81ee51cd629b818bbedac`  
		Last Modified: Tue, 08 Aug 2023 19:46:59 GMT  
		Size: 45.2 MB (45190380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f50935a8980aae448b158b40171ce38beb0eaaac6885c4f54cce54e91111d`  
		Last Modified: Tue, 08 Aug 2023 19:46:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f0a93a82bda1755bff5d618fe66a84d7a66aa14b6a354e0cba1523e594c088`  
		Last Modified: Tue, 08 Aug 2023 19:46:53 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639e7d04c7fcfd6d278fdb6171706187682498b6aad235b3be91c12e45773392`  
		Last Modified: Tue, 08 Aug 2023 22:48:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3b7bd731e85eb85c198d423b04043afc9b9cce07457cbf429bb4b15d8ed8ad`  
		Last Modified: Tue, 08 Aug 2023 22:48:07 GMT  
		Size: 12.2 MB (12228902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af603f750f5e7cfe5b27da830d07f503d9be1b0e3f13b58da82aa4e4f3411d9`  
		Last Modified: Tue, 08 Aug 2023 22:48:07 GMT  
		Size: 455.9 KB (455942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe05621ee5db996e72edb85769de4bed2efc30d470d854db152111a36dba18c`  
		Last Modified: Tue, 08 Aug 2023 22:48:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; ppc64le

```console
$ docker pull tomcat@sha256:91bd24a78721135393063ebac59c2fc842628499307215e88c7034a0477271e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104504424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2ea11c43030d1ad5b8834baf9de810efb96296cc566dd84b5ca136ca69be88`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 00:18:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 00:18:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 00:18:19 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:19:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:21:25 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:22:37 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:22:38 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:22:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 21:03:30 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 21:03:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:03:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 21:03:32 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 21:03:33 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:03:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:03:33 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 08 Aug 2023 21:03:34 GMT
ENV TOMCAT_MAJOR=10
# Tue, 08 Aug 2023 21:03:34 GMT
ENV TOMCAT_VERSION=10.1.11
# Tue, 08 Aug 2023 21:03:36 GMT
ENV TOMCAT_SHA512=ad754aa695898cf8af5b64f4e29da7013fb39f808a90fa0e030228680a17c01b10bb0904762417ebac99b075947e4ea26f2f22f5da2aa4e399237468b76fa4fb
# Tue, 08 Aug 2023 21:03:37 GMT
COPY dir:97e43246b140837205d24d470cdb0ca267da32adcb9d786ecc06edc6ad182fc8 in /usr/local/tomcat 
# Tue, 08 Aug 2023 21:03:49 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:03:53 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 21:03:53 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:15:10 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:15:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2f5a106d782ce62a5cf92c2a7f53d1b6067d5198e321d1c74bf914ae7b208f`  
		Last Modified: Tue, 08 Aug 2023 19:28:59 GMT  
		Size: 13.8 MB (13770640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165a80cbdb7b61d7a95bcc244443e23a3069edb8cf8f0552be6581117a7fb3c3`  
		Last Modified: Tue, 08 Aug 2023 19:33:10 GMT  
		Size: 42.3 MB (42295309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad547ccf5a7181bed1599a10c0225336c8544a8fb637b97dd9c901fcb54fa33e`  
		Last Modified: Tue, 08 Aug 2023 19:32:59 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1943e298b8799c3be0cd6731d681795316d3b4a21ec0e099e765625a3a2eada`  
		Last Modified: Tue, 08 Aug 2023 19:32:59 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8629aea934a23d6e284a17d7018a2034b72174ef59389e5fc3ba0b56b6d500be`  
		Last Modified: Tue, 08 Aug 2023 21:40:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db3082073b3f2d82f27c65e92a1a86c70ca0cfa94c11d89f18106e262ff164f`  
		Last Modified: Tue, 08 Aug 2023 21:40:37 GMT  
		Size: 12.2 MB (12238954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54e25971ebb01a52e87a0640891af7ea67727937e7a49f4bffb4be5e541937f`  
		Last Modified: Tue, 08 Aug 2023 21:40:35 GMT  
		Size: 486.9 KB (486919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb4eb011579c1aed69dc5c07f0f9a621d7881e199ed7be31f2a361541129174`  
		Last Modified: Tue, 08 Aug 2023 21:40:35 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; s390x

```console
$ docker pull tomcat@sha256:df27588e6461c5dca357ccb1adec36236ffcfa085a43725678fe9bdff8ee1a2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94947419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada24323334b0d400aa5b1a8e2c20b85e20a1f4c0f58fdcd8ec69936ca262c7f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 16:24:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:24:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:42:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:42:56 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:43:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:43:36 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:43:36 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:43:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 20:09:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 20:09:17 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:09:18 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 20:09:18 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 20:09:18 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 20:09:18 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 20:09:18 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 08 Aug 2023 20:09:18 GMT
ENV TOMCAT_MAJOR=10
# Tue, 08 Aug 2023 20:09:18 GMT
ENV TOMCAT_VERSION=10.1.11
# Tue, 08 Aug 2023 20:09:18 GMT
ENV TOMCAT_SHA512=ad754aa695898cf8af5b64f4e29da7013fb39f808a90fa0e030228680a17c01b10bb0904762417ebac99b075947e4ea26f2f22f5da2aa4e399237468b76fa4fb
# Tue, 08 Aug 2023 20:09:19 GMT
COPY dir:d1d3011434b4a5eddd2c15c07c70f979359940bcc03a33deabb0a973a1220c72 in /usr/local/tomcat 
# Tue, 08 Aug 2023 20:09:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 20:09:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 20:09:23 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:05:43 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:05:43 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c50c1c8dac118ab286a3daca746c31d4f16f57d4a01f96c6538eeca886cafd`  
		Last Modified: Tue, 08 Aug 2023 19:46:30 GMT  
		Size: 13.0 MB (12981935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d424bed4049f5cf52f12697efc3fe523bc4707130adfb89345709da2e4e8ca9`  
		Last Modified: Tue, 08 Aug 2023 19:47:11 GMT  
		Size: 40.6 MB (40631193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3def242509c79c9ab5ad5c0d8bc6f938bccc2cb6bb3c44cb5f26670034581ef`  
		Last Modified: Tue, 08 Aug 2023 19:47:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc77f682b0e12c84d69e1ab6735b311b61f235d127d06a7b80d50e2e2215bce1`  
		Last Modified: Tue, 08 Aug 2023 19:47:05 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d999e748c081631ed8d85c88cc3d5046200a1f8aeb54d2fb5f22a237054702`  
		Last Modified: Tue, 08 Aug 2023 20:18:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcf3c376ed4d3a3ff352dfb5e265eae512e6329cd3ec51746f4ddce2c2ddfd2`  
		Last Modified: Tue, 08 Aug 2023 20:18:40 GMT  
		Size: 12.2 MB (12230199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff29dff2e817760cb91239462b5238efc2a043b87ecfb3b6b3199085d15bed6a`  
		Last Modified: Tue, 08 Aug 2023 20:18:40 GMT  
		Size: 457.3 KB (457267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37ab0f5e1265e17a2f0fed970047a062fc858c84d8acbc0d4bd8b07f7d6f2b6`  
		Last Modified: Tue, 08 Aug 2023 20:18:39 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
