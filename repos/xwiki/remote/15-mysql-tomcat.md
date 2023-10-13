## `xwiki:15-mysql-tomcat`

```console
$ docker pull xwiki@sha256:e3bddf36e6d345a39645d9e95358a01dc4a0275d9f8903aabf5bb4893b0437de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:26006a0c10f743ec6f660eacd380515131f5dfb5a0cac7024d2e973e25978c6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.2 MB (592190697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2767c84cfbed1ed858ea7ca0b22b50da0b93b8d8b0b4da108ecd147b5495634d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Tue, 03 Oct 2023 09:36:41 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 03 Oct 2023 09:36:42 GMT
ENV TOMCAT_MAJOR=9
# Tue, 03 Oct 2023 09:36:42 GMT
ENV TOMCAT_VERSION=9.0.80
# Tue, 03 Oct 2023 09:36:42 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Tue, 03 Oct 2023 09:36:42 GMT
COPY dir:6c825f167724fd169268039dada74938279a848f3780e636938f06347c3f4ef4 in /usr/local/tomcat 
# Tue, 03 Oct 2023 09:36:46 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:36:48 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 03 Oct 2023 09:36:48 GMT
EXPOSE 8080
# Tue, 03 Oct 2023 09:36:48 GMT
ENTRYPOINT []
# Tue, 03 Oct 2023 09:36:48 GMT
CMD ["catalina.sh" "run"]
# Tue, 03 Oct 2023 11:41:44 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Tue, 03 Oct 2023 11:41:44 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Tue, 03 Oct 2023 11:41:44 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Tue, 03 Oct 2023 11:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Tue, 03 Oct 2023 11:41:44 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Tue, 03 Oct 2023 11:41:44 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Tue, 03 Oct 2023 11:45:26 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 11:45:27 GMT
ENV XWIKI_VERSION=15.8
# Tue, 03 Oct 2023 11:45:28 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.8
# Tue, 03 Oct 2023 11:45:28 GMT
ENV XWIKI_DOWNLOAD_SHA256=359e44485615722ab533559ec3e3334197a10935e4dfa6fc872b93d1447475fc
# Tue, 03 Oct 2023 11:46:07 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 03 Oct 2023 11:46:07 GMT
ENV MYSQL_JDBC_VERSION=8.1.0
# Tue, 03 Oct 2023 11:46:08 GMT
ENV MYSQL_JDBC_SHA256=e2e657e9c5ebe06a73485c9739ebd8a18e7bebb852a58d0da287da850beca1c7
# Tue, 03 Oct 2023 11:46:08 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.1.0
# Tue, 03 Oct 2023 11:46:08 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.1.0.jar
# Tue, 03 Oct 2023 11:46:08 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.1.0.jar
# Tue, 03 Oct 2023 11:46:09 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 03 Oct 2023 11:46:09 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 03 Oct 2023 11:46:09 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 03 Oct 2023 11:46:10 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 03 Oct 2023 11:46:10 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 03 Oct 2023 11:46:10 GMT
VOLUME [/usr/local/xwiki]
# Tue, 03 Oct 2023 11:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 11:46:10 GMT
CMD ["xwiki"]
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
	-	`sha256:bfcd3780c6b55ffa197b91db2f6582bb3f2aaf73b18c990bb53c0e53ecba6caf`  
		Last Modified: Tue, 03 Oct 2023 09:47:05 GMT  
		Size: 12.3 MB (12285252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60ae46296d1efa5f40779556cf4e7f0452061a8dd0a8a75302bcb447b4976c2`  
		Last Modified: Tue, 03 Oct 2023 09:47:04 GMT  
		Size: 455.7 KB (455665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e491498a7ccb4ffa24cff2489f399d677fd12090c40e44903ffd64d4ba60a09a`  
		Last Modified: Tue, 03 Oct 2023 09:47:04 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07fcbf8045a011156660812b6b5b96e6dfee9f83d149032ff9137fd49e9aa46`  
		Last Modified: Tue, 03 Oct 2023 11:52:15 GMT  
		Size: 178.4 MB (178357813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d42a59e89819017e9e3cedd942467bb142db8e515f6f8d196a217e63608556f`  
		Last Modified: Tue, 03 Oct 2023 11:52:08 GMT  
		Size: 308.5 MB (308522694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9db6036ccd3f2f69bc318129fe3f111999d579ecb450271405ceaf6316e622`  
		Last Modified: Tue, 03 Oct 2023 11:51:50 GMT  
		Size: 2.3 MB (2347562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c272a1f4ae8e600e0e02ea0ffcc66ed39b279f93a1ba2e3f6caa92beaaffbc`  
		Last Modified: Tue, 03 Oct 2023 11:51:50 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d35fe32a3b9b4aaa767f8f199e93241afd819a692bce8eebd5569d18987b03`  
		Last Modified: Tue, 03 Oct 2023 11:51:50 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be08989ad8b25e2d6366865aacbb00ac68d504a9c53d232d28b934fc297b0bc1`  
		Last Modified: Tue, 03 Oct 2023 11:51:50 GMT  
		Size: 6.3 KB (6318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2c32788f97a2348a14b53feaf163d6e8874f01b8fb44b7020889df588ee33f`  
		Last Modified: Tue, 03 Oct 2023 11:51:50 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:eb96b045280512954ad639619141506c0d5bd20012e9aa163dd6a3740ee6a760
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.9 MB (583930976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ec8f767d675d19e8645ef75eb6ce90053efef6e8888fe2550e10129252d1a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Tue, 03 Oct 2023 07:51:23 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 03 Oct 2023 07:51:23 GMT
ENV TOMCAT_MAJOR=9
# Fri, 13 Oct 2023 00:21:10 GMT
ENV TOMCAT_VERSION=9.0.81
# Fri, 13 Oct 2023 00:21:10 GMT
ENV TOMCAT_SHA512=919957776addb26570f4c4cc2a65159409baf6b5851b3524cc07ffb7ede289ce00f454e547d309eb772e543eea0956201067e0a7b4627d182eff7e2ce042e298
# Fri, 13 Oct 2023 00:21:10 GMT
COPY dir:780a5ea2277ee7b7a4224ff98e735f9335b57508576452554c06350ed6015658 in /usr/local/tomcat 
# Fri, 13 Oct 2023 00:21:14 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:21:15 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 13 Oct 2023 00:21:15 GMT
EXPOSE 8080
# Fri, 13 Oct 2023 00:21:15 GMT
ENTRYPOINT []
# Fri, 13 Oct 2023 00:21:15 GMT
CMD ["catalina.sh" "run"]
# Fri, 13 Oct 2023 02:10:23 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 13 Oct 2023 02:10:23 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 13 Oct 2023 02:10:23 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 13 Oct 2023 02:10:23 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 13 Oct 2023 02:10:23 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 13 Oct 2023 02:10:23 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 13 Oct 2023 02:12:24 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:12:27 GMT
ENV XWIKI_VERSION=15.8
# Fri, 13 Oct 2023 02:12:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.8
# Fri, 13 Oct 2023 02:12:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=359e44485615722ab533559ec3e3334197a10935e4dfa6fc872b93d1447475fc
# Fri, 13 Oct 2023 02:13:08 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 13 Oct 2023 02:13:10 GMT
ENV MYSQL_JDBC_VERSION=8.1.0
# Fri, 13 Oct 2023 02:13:10 GMT
ENV MYSQL_JDBC_SHA256=e2e657e9c5ebe06a73485c9739ebd8a18e7bebb852a58d0da287da850beca1c7
# Fri, 13 Oct 2023 02:13:11 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.1.0
# Fri, 13 Oct 2023 02:13:11 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.1.0.jar
# Fri, 13 Oct 2023 02:13:11 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.1.0.jar
# Fri, 13 Oct 2023 02:13:11 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Fri, 13 Oct 2023 02:13:12 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 13 Oct 2023 02:13:12 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 13 Oct 2023 02:13:12 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 13 Oct 2023 02:13:12 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 13 Oct 2023 02:13:12 GMT
VOLUME [/usr/local/xwiki]
# Fri, 13 Oct 2023 02:13:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 02:13:12 GMT
CMD ["xwiki"]
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
	-	`sha256:3fdc89704c8360e1cf43907bb9a97a283582b1d8f6b0afa620d464d9fc5bc687`  
		Last Modified: Fri, 13 Oct 2023 00:45:04 GMT  
		Size: 12.3 MB (12323632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11143617fb5366012e499899ef5146a79be3846ba99a71f427dc9c50e5f08d`  
		Last Modified: Fri, 13 Oct 2023 00:45:03 GMT  
		Size: 455.9 KB (455934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2352884ee03f9e4fe1f93282d89f0876eb5b04bf85cdc124917597e9fd83aafb`  
		Last Modified: Fri, 13 Oct 2023 00:45:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dabb03f96e1877e97473c5711615c25b98fa6c2aedd9033b8f957c7aafb829`  
		Last Modified: Fri, 13 Oct 2023 02:18:56 GMT  
		Size: 173.8 MB (173841139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7b9296f65363ffff3fdba181c19c0ac2a03171ddc075459cc1584c57c8ae42`  
		Last Modified: Fri, 13 Oct 2023 02:18:58 GMT  
		Size: 308.5 MB (308522718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb7bd12a77efe33b04ab2cd9765f5fd1f4884feae0c76f5b57bb5644afb5d7f`  
		Last Modified: Fri, 13 Oct 2023 02:18:38 GMT  
		Size: 2.3 MB (2347564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f0ac4ca37d18d2e9fcca147180e9ea46968c9fc4fdd4007f0415b25ce8d352`  
		Last Modified: Fri, 13 Oct 2023 02:18:38 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7727c5384daa442b51a8c8417042adc50779dc30b07200bddc35285062a7ad5`  
		Last Modified: Fri, 13 Oct 2023 02:18:38 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f3b58a77a864acf8c98b71bafd4d98fa89c40e992f53b6728bddca3a084a27`  
		Last Modified: Fri, 13 Oct 2023 02:18:38 GMT  
		Size: 6.3 KB (6319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d134215152d16a66568c3b53221d3b978262376ba38d173b708aea59ddc535ba`  
		Last Modified: Fri, 13 Oct 2023 02:18:38 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
