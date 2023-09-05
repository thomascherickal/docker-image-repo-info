## `xwiki:lts-mysql-tomcat`

```console
$ docker pull xwiki@sha256:9b6bf8a79a9df454be2b1b9849f781b02ae005b009d7a97ca84285879ab7350e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:e90f9b70fb6eb1aa1ddb1d360c4d9e9efecdfc3302c64750833e3e1ad24d48b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.7 MB (592693429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b5ac6588b62d85b0423fabbdcf4ba193def9517d98a191b6d10e25be81caa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:37:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 00:37:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 00:37:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Sep 2023 00:37:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:38:36 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Sat, 02 Sep 2023 00:39:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Sep 2023 00:39:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 02 Sep 2023 00:39:05 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Sep 2023 00:39:05 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Sep 2023 03:43:14 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Sep 2023 03:43:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 03:43:15 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Sep 2023 03:43:15 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Sep 2023 03:43:15 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Sep 2023 03:43:15 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Sep 2023 03:44:59 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 02 Sep 2023 03:44:59 GMT
ENV TOMCAT_MAJOR=9
# Sat, 02 Sep 2023 03:44:59 GMT
ENV TOMCAT_VERSION=9.0.80
# Sat, 02 Sep 2023 03:44:59 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Sat, 02 Sep 2023 03:44:59 GMT
COPY dir:d7e211ba43c9ae41c4526bf9dad571066be23b7faa3126c3d0bf989be5e2e4ea in /usr/local/tomcat 
# Sat, 02 Sep 2023 03:45:04 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 03:45:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Sep 2023 03:45:05 GMT
EXPOSE 8080
# Sat, 02 Sep 2023 03:45:05 GMT
ENTRYPOINT []
# Sat, 02 Sep 2023 03:45:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Sep 2023 08:50:02 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 02 Sep 2023 08:50:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 02 Sep 2023 08:50:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 02 Sep 2023 08:50:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 02 Sep 2023 08:50:03 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 02 Sep 2023 08:50:03 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 02 Sep 2023 08:51:41 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 05 Sep 2023 22:34:01 GMT
ENV XWIKI_VERSION=14.10.16
# Tue, 05 Sep 2023 22:34:01 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.16
# Tue, 05 Sep 2023 22:34:01 GMT
ENV XWIKI_DOWNLOAD_SHA256=621bdbabe3a462e2e1ef8b8fd9629ef0f8bbea975719c6873de3f90653ede656
# Tue, 05 Sep 2023 22:34:40 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 05 Sep 2023 22:34:40 GMT
ENV MYSQL_JDBC_VERSION=8.1.0
# Tue, 05 Sep 2023 22:34:41 GMT
ENV MYSQL_JDBC_SHA256=e2e657e9c5ebe06a73485c9739ebd8a18e7bebb852a58d0da287da850beca1c7
# Tue, 05 Sep 2023 22:34:41 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.1.0
# Tue, 05 Sep 2023 22:34:41 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.1.0.jar
# Tue, 05 Sep 2023 22:34:41 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.1.0.jar
# Tue, 05 Sep 2023 22:34:42 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 05 Sep 2023 22:34:42 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 05 Sep 2023 22:34:42 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 05 Sep 2023 22:34:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 05 Sep 2023 22:34:42 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 05 Sep 2023 22:34:43 GMT
VOLUME [/usr/local/xwiki]
# Tue, 05 Sep 2023 22:34:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 22:34:43 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274fb0278626020650ff7c358074255903c792176a61a1ebce3055ba27e11436`  
		Last Modified: Sat, 02 Sep 2023 00:41:34 GMT  
		Size: 12.9 MB (12902882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00346ef46b0fe8a50b11fd9621a92a596760afe94bc7f1941e884d97e4b239a1`  
		Last Modified: Sat, 02 Sep 2023 00:42:41 GMT  
		Size: 46.9 MB (46864483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e407e98debb8151066db1e98639d0fc3cfe04dab507e3d032537a64ecd85d4`  
		Last Modified: Sat, 02 Sep 2023 00:42:34 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4075bbc4ec0f48ded2ad33e229d3a85fd6c61f3acf35c85fd6a6ce8fd1dd44b7`  
		Last Modified: Sat, 02 Sep 2023 00:42:34 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0760623340fc44750aa3df57005e382ac8671c2492e6f7f6f89ee0ab6b5b4cd`  
		Last Modified: Sat, 02 Sep 2023 03:52:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0303afc506abfa7a02c475d50c1fe0b3dbfd7a5335bd16d58e8bd16022579a26`  
		Last Modified: Sat, 02 Sep 2023 03:54:17 GMT  
		Size: 12.3 MB (12285235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed7f0b9c144157fea85e22faf7262fc3aec6b708240de7524e48e8d0efb7c48`  
		Last Modified: Sat, 02 Sep 2023 03:54:16 GMT  
		Size: 455.6 KB (455564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571d84ab4f37d729996290f14196965ed60f9d24192faf3f4a011fb5b0d0edc9`  
		Last Modified: Sat, 02 Sep 2023 03:54:16 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8243ab0f5c5ff2e1e4219296ff13e241ac0ba132cb2aa86e0c20d9d52435b6fa`  
		Last Modified: Sat, 02 Sep 2023 08:58:24 GMT  
		Size: 178.4 MB (178356623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d50d035fa749cdc1c9b132d0c59e83a2db29eea5f5a53b6390bc7083b67fa7`  
		Last Modified: Tue, 05 Sep 2023 22:36:44 GMT  
		Size: 309.0 MB (309028727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dd43d5b5afb55b48256ab1726790248561170d5e5d5c93bc3f013a53752f6b`  
		Last Modified: Tue, 05 Sep 2023 22:36:27 GMT  
		Size: 2.3 MB (2347565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedf6f7858d8525393434e39769c6540bc5b36037e32abfe50810676d13dd75e`  
		Last Modified: Tue, 05 Sep 2023 22:36:26 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62e74f905350eba6ed8f9bd6e449f8e75d373b5c06be0d870c135a361b02ea4`  
		Last Modified: Tue, 05 Sep 2023 22:36:26 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8d9ab2c7ccf8bcc446ee2a9c43ec767559e5860bbf6d11d4524130317d3ed0`  
		Last Modified: Tue, 05 Sep 2023 22:36:26 GMT  
		Size: 6.0 KB (6018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17de9251784059390daa96b12688b4c56bcb6b1641c3d085919dd3e019e34c5`  
		Last Modified: Tue, 05 Sep 2023 22:36:26 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6d9e8e0ab4a2f157296c58471c813d88e95e99e53ab0b80cf2e8eec3f417a05a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.0 MB (583957497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7cf48dc59f4caab1d99f07e1d406fe0e9322d340ce42a82605d231f2879f28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:28:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 01 Sep 2023 23:28:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 23:28:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Sep 2023 23:29:07 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:29:31 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 01 Sep 2023 23:29:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 01 Sep 2023 23:29:56 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 01 Sep 2023 23:29:56 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Sep 2023 23:29:56 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Sep 2023 02:02:10 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Sep 2023 02:02:10 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 02:02:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Sep 2023 02:02:10 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Sep 2023 02:02:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Sep 2023 02:02:11 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Sep 2023 02:03:38 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 02 Sep 2023 02:03:38 GMT
ENV TOMCAT_MAJOR=9
# Sat, 02 Sep 2023 02:03:38 GMT
ENV TOMCAT_VERSION=9.0.80
# Sat, 02 Sep 2023 02:03:38 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Sat, 02 Sep 2023 02:03:38 GMT
COPY dir:b31dee11dfcfa943f9d76689217cc078d150ddd034da36a15450915bfcd1e5f4 in /usr/local/tomcat 
# Sat, 02 Sep 2023 02:03:42 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 02:03:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Sep 2023 02:03:43 GMT
EXPOSE 8080
# Sat, 02 Sep 2023 02:03:43 GMT
ENTRYPOINT []
# Sat, 02 Sep 2023 02:03:43 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Sep 2023 04:06:11 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 02 Sep 2023 04:06:11 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 02 Sep 2023 04:06:11 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 02 Sep 2023 04:06:11 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 02 Sep 2023 04:06:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 02 Sep 2023 04:06:12 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 02 Sep 2023 04:07:50 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 04:10:16 GMT
ENV XWIKI_VERSION=14.10.15
# Sat, 02 Sep 2023 04:10:16 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.15
# Sat, 02 Sep 2023 04:10:16 GMT
ENV XWIKI_DOWNLOAD_SHA256=7deecd23f9c477b06a58027948d63097467f9b3bfc17cea21061395bf0e1340d
# Sat, 02 Sep 2023 04:10:55 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 02 Sep 2023 04:10:58 GMT
ENV MYSQL_JDBC_VERSION=8.1.0
# Sat, 02 Sep 2023 04:10:58 GMT
ENV MYSQL_JDBC_SHA256=e2e657e9c5ebe06a73485c9739ebd8a18e7bebb852a58d0da287da850beca1c7
# Sat, 02 Sep 2023 04:10:58 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.1.0
# Sat, 02 Sep 2023 04:10:58 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.1.0.jar
# Sat, 02 Sep 2023 04:10:58 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.1.0.jar
# Sat, 02 Sep 2023 04:10:59 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Sat, 02 Sep 2023 04:10:59 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 02 Sep 2023 04:10:59 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 02 Sep 2023 04:10:59 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 02 Sep 2023 04:11:00 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 02 Sep 2023 04:11:00 GMT
VOLUME [/usr/local/xwiki]
# Sat, 02 Sep 2023 04:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Sep 2023 04:11:00 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8624f6e9281a23943755ff078ce7c91b6b23aa7887445c9345622a3fdb3f32`  
		Last Modified: Fri, 01 Sep 2023 23:31:56 GMT  
		Size: 12.8 MB (12845046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8091da28544a8e03ba46a693ac64626bcc4e76cfab0a944e8ae8544db91ebf09`  
		Last Modified: Fri, 01 Sep 2023 23:33:00 GMT  
		Size: 45.2 MB (45190521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032cd2d33c4b8328ceab6cc35be2ddd3fc5aff61faec4139f21b20ac8f4b0f93`  
		Last Modified: Fri, 01 Sep 2023 23:32:55 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee0abc3216130a928fe9ff4ba83fbc16a52aa9e0797392a0b28bb3c06a1111a`  
		Last Modified: Fri, 01 Sep 2023 23:32:55 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa49100ae34321a6593b295c165c1ca1971e3cc06c6c398601694798af99555`  
		Last Modified: Sat, 02 Sep 2023 02:10:18 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6b7a59e3eeb1627b9bbfdda6fe5f86426393f9dbc91efba9ca722ff1307d43`  
		Last Modified: Sat, 02 Sep 2023 02:12:10 GMT  
		Size: 12.3 MB (12291671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e7b0a6a0c6c98c36024efb08f8a6d18a254f28eb2827e89edf6e1d317d39ca`  
		Last Modified: Sat, 02 Sep 2023 02:12:09 GMT  
		Size: 456.8 KB (456847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270f488e7aecc8a40caa754cbffa3a8854b0c4f8dcc34eb09e3a505b22ebbed1`  
		Last Modified: Sat, 02 Sep 2023 02:12:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0f291c51328d7044de62c9f8de2c8863b150fbecb842a556f8a94757ec2adc`  
		Last Modified: Sat, 02 Sep 2023 04:14:14 GMT  
		Size: 173.4 MB (173396123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9429dd7ba95652285b4f140367d1e7c66b28e13091bc63d6e038788bed5f72f6`  
		Last Modified: Sat, 02 Sep 2023 04:16:06 GMT  
		Size: 309.0 MB (309023385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7742878228e26b2bca678d46edc39123cc67917db5571acde2581766bf1ef96e`  
		Last Modified: Sat, 02 Sep 2023 04:15:51 GMT  
		Size: 2.3 MB (2347563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7362cb812d9a29360760bd2246c6570e47f2f95ce6b97990575a69c62b8ddf41`  
		Last Modified: Sat, 02 Sep 2023 04:15:51 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660a3de00c4fdc36bce797a5955d4560fa5a7fa3b361409fa37d143d64acb1c4`  
		Last Modified: Sat, 02 Sep 2023 04:15:51 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ea5741bc1142e4c646ae69b0edaef757279de75368664474fde58d5d4d51e0`  
		Last Modified: Sat, 02 Sep 2023 04:15:51 GMT  
		Size: 6.0 KB (6014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a701e1f3857a3cec8b7505a642ab9fe38024f2219e404c671b752f8fc1ac658c`  
		Last Modified: Sat, 02 Sep 2023 04:15:51 GMT  
		Size: 2.5 KB (2501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
