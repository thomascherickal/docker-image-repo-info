## `xwiki:14-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:3f01496a2e3d3a08c5cd004bc61c8a708f7e06540c5965663ec602b375b789d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:b326bcc3312d20337931bd7f10ebfc828813a5f4902032531dc56baa1c5a6ab2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **598.4 MB (598385323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee83eb4777f0e13b36e9685ef92308449a7bb454149ddf93f44eef3e3733a80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:51:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 05:51:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 05:51:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:27:44 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:27:44 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:29:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:29:19 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:29:19 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:29:19 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 31 Oct 2023 03:37:14 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 31 Oct 2023 03:37:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 03:37:14 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 31 Oct 2023 03:37:14 GMT
WORKDIR /usr/local/tomcat
# Tue, 31 Oct 2023 03:37:14 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 31 Oct 2023 03:37:14 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 31 Oct 2023 03:39:32 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 31 Oct 2023 03:39:32 GMT
ENV TOMCAT_MAJOR=9
# Tue, 31 Oct 2023 03:39:32 GMT
ENV TOMCAT_VERSION=9.0.82
# Tue, 31 Oct 2023 03:39:32 GMT
ENV TOMCAT_SHA512=2b13f11f4e0d0b9aee667c256c6ea5d2853b067e8b7e8293f117da050d3833fda8aa9d9ad278bd12fb7fbf0825108c7d0384509f44c05f9bad73eb099cfaa128
# Tue, 31 Oct 2023 03:39:33 GMT
COPY dir:4fdd96615cb958335f3b12700d702e3ffcee07613ee616e5456e799e6dfe0b52 in /usr/local/tomcat 
# Tue, 31 Oct 2023 03:39:38 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Oct 2023 03:39:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 31 Oct 2023 03:39:39 GMT
EXPOSE 8080
# Tue, 31 Oct 2023 03:39:39 GMT
ENTRYPOINT []
# Tue, 31 Oct 2023 03:39:39 GMT
CMD ["catalina.sh" "run"]
# Thu, 09 Nov 2023 20:22:33 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Thu, 09 Nov 2023 20:22:33 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Thu, 09 Nov 2023 20:22:33 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Thu, 09 Nov 2023 20:22:33 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Thu, 09 Nov 2023 20:22:33 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Thu, 09 Nov 2023 20:22:33 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Thu, 09 Nov 2023 20:24:13 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Thu, 09 Nov 2023 20:24:14 GMT
ENV XWIKI_VERSION=14.10.19
# Thu, 09 Nov 2023 20:24:14 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.19
# Thu, 09 Nov 2023 20:24:14 GMT
ENV XWIKI_DOWNLOAD_SHA256=14b88314f9af3c122e3329d13ad2a8a473a774fa1bc8b5b96d08bbf36e56c453
# Thu, 09 Nov 2023 20:24:57 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 09 Nov 2023 20:26:35 GMT
ENV MARIADB_JDBC_VERSION=3.2.0
# Thu, 09 Nov 2023 20:26:35 GMT
ENV MARIADB_JDBC_SHA256=adf9df10bc9b2a137def36d6a495812258f430d4a8f7946727c61558e6c73941
# Thu, 09 Nov 2023 20:26:35 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.2.0
# Thu, 09 Nov 2023 20:26:36 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.2.0.jar
# Thu, 09 Nov 2023 20:26:36 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.2.0.jar
# Thu, 09 Nov 2023 20:26:36 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Thu, 09 Nov 2023 20:26:37 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 09 Nov 2023 20:26:37 GMT
COPY file:eb83c176c15b3f58dfe8a9489b3339583ffd67428f115d02fc75fd828ba98995 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 09 Nov 2023 20:26:37 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 09 Nov 2023 20:26:37 GMT
COPY file:999bc8865c34789d8e469cd12cf9ae2fc932b27d4508dd5ae18997c8eca23a9b in /usr/local/bin/docker-entrypoint.sh 
# Thu, 09 Nov 2023 20:26:37 GMT
VOLUME [/usr/local/xwiki]
# Thu, 09 Nov 2023 20:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 20:26:38 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4452d37e1e46888f8dbbf8283d09e03f1bec00021532334441fe00c95aa8b15`  
		Last Modified: Mon, 30 Oct 2023 23:36:06 GMT  
		Size: 17.5 MB (17454768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae6cc00f059e812c753a4a45b4a388d14bb714a104ec8b33c31436807f31055`  
		Last Modified: Mon, 30 Oct 2023 23:37:50 GMT  
		Size: 47.1 MB (47149391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaec5da5e638ca5d7247c8697d0721bdac4826945748d0239718f23f657abc5`  
		Last Modified: Mon, 30 Oct 2023 23:37:44 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7dcc43773c1bcab928db7ca63abd5a20c525148ae1b63c03bfdcdef7e03153`  
		Last Modified: Mon, 30 Oct 2023 23:37:44 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6729bb2516f9ee1f23d3c6b1a60b651eb413c43b62cdc554de84df2590085216`  
		Last Modified: Tue, 31 Oct 2023 03:53:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9168864721356533b0669f4446b3b9f62f971b648862ea49c25c758117374986`  
		Last Modified: Tue, 31 Oct 2023 03:56:21 GMT  
		Size: 12.3 MB (12315466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541fb3b6d3fc04d699b424c3d27f1fd761b49c3a2f8635c10bfc6950d3504c5a`  
		Last Modified: Tue, 31 Oct 2023 03:56:21 GMT  
		Size: 3.0 MB (2970840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333283eafa5961340497c34e61f546f2485c7097991f05509d2f7c8b1709e357`  
		Last Modified: Tue, 31 Oct 2023 03:56:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4751ba0c4469c8db469596ba627419d66da68884d05c8aec103678165c9831b3`  
		Last Modified: Thu, 09 Nov 2023 20:27:49 GMT  
		Size: 178.4 MB (178359341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404ff07441357591740fed9743b869d603913dddacb3859ef74936e861206090`  
		Last Modified: Thu, 09 Nov 2023 20:27:41 GMT  
		Size: 309.1 MB (309079698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81aad63bcb55e9e107f22154bb6e6d135d0743e007f1063cdb3959830b66be7`  
		Last Modified: Thu, 09 Nov 2023 20:29:01 GMT  
		Size: 603.4 KB (603393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883289b339d5f0e6c9e9ac716814fdfaa07e75235d1c3e50bb0543d3480d3e8e`  
		Last Modified: Thu, 09 Nov 2023 20:29:00 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a49d5826845c224281ff6fe467bfc66dbf1e737e5011f3d0a1261ca724b21e`  
		Last Modified: Thu, 09 Nov 2023 20:29:00 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bca33231f2bbc04758280b2ee5a2fa92e41569f912ec4a69a268a6722a80cd`  
		Last Modified: Thu, 09 Nov 2023 20:29:00 GMT  
		Size: 6.0 KB (6016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d3ac1148d28621699b8ce6ba5045d329f8671aa746c52cfa4729467db31e96`  
		Last Modified: Thu, 09 Nov 2023 20:29:00 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:4de209b5ec50b8a3bcedcc1d596c0bf2206a30698e38f318aeedeede2d321aa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.1 MB (592099337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f39d1298d369cfe954c03429aea86a966956c40765068c487b293faf04a687`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:44:05 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:44:05 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:45:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:45:35 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:45:35 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:45:35 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 31 Oct 2023 02:56:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 31 Oct 2023 02:56:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 02:56:14 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 31 Oct 2023 02:56:14 GMT
WORKDIR /usr/local/tomcat
# Tue, 31 Oct 2023 02:56:14 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 31 Oct 2023 02:56:14 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 31 Oct 2023 02:58:17 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 31 Oct 2023 02:58:17 GMT
ENV TOMCAT_MAJOR=9
# Tue, 31 Oct 2023 02:58:17 GMT
ENV TOMCAT_VERSION=9.0.82
# Tue, 31 Oct 2023 02:58:17 GMT
ENV TOMCAT_SHA512=2b13f11f4e0d0b9aee667c256c6ea5d2853b067e8b7e8293f117da050d3833fda8aa9d9ad278bd12fb7fbf0825108c7d0384509f44c05f9bad73eb099cfaa128
# Tue, 31 Oct 2023 02:58:17 GMT
COPY dir:065ce3e827a9660f642ca26c02331e7158625b52fb53779a789b9b8cd11605e1 in /usr/local/tomcat 
# Tue, 31 Oct 2023 02:58:21 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Oct 2023 02:58:22 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 31 Oct 2023 02:58:22 GMT
EXPOSE 8080
# Tue, 31 Oct 2023 02:58:22 GMT
ENTRYPOINT []
# Tue, 31 Oct 2023 02:58:23 GMT
CMD ["catalina.sh" "run"]
# Thu, 09 Nov 2023 20:51:58 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Thu, 09 Nov 2023 20:51:58 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Thu, 09 Nov 2023 20:51:58 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Thu, 09 Nov 2023 20:51:58 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Thu, 09 Nov 2023 20:51:58 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Thu, 09 Nov 2023 20:51:58 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Thu, 09 Nov 2023 20:54:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Thu, 09 Nov 2023 20:54:06 GMT
ENV XWIKI_VERSION=14.10.19
# Thu, 09 Nov 2023 20:54:06 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.19
# Thu, 09 Nov 2023 20:54:06 GMT
ENV XWIKI_DOWNLOAD_SHA256=14b88314f9af3c122e3329d13ad2a8a473a774fa1bc8b5b96d08bbf36e56c453
# Thu, 09 Nov 2023 20:54:48 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 09 Nov 2023 20:56:28 GMT
ENV MARIADB_JDBC_VERSION=3.2.0
# Thu, 09 Nov 2023 20:56:28 GMT
ENV MARIADB_JDBC_SHA256=adf9df10bc9b2a137def36d6a495812258f430d4a8f7946727c61558e6c73941
# Thu, 09 Nov 2023 20:56:28 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.2.0
# Thu, 09 Nov 2023 20:56:28 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.2.0.jar
# Thu, 09 Nov 2023 20:56:28 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.2.0.jar
# Thu, 09 Nov 2023 20:56:29 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Thu, 09 Nov 2023 20:56:29 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 09 Nov 2023 20:56:29 GMT
COPY file:eb83c176c15b3f58dfe8a9489b3339583ffd67428f115d02fc75fd828ba98995 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 09 Nov 2023 20:56:30 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 09 Nov 2023 20:56:30 GMT
COPY file:999bc8865c34789d8e469cd12cf9ae2fc932b27d4508dd5ae18997c8eca23a9b in /usr/local/bin/docker-entrypoint.sh 
# Thu, 09 Nov 2023 20:56:30 GMT
VOLUME [/usr/local/xwiki]
# Thu, 09 Nov 2023 20:56:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 20:56:30 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f494a0917249ff640404cd9965fcd6a5ed5b7725fc21ff44518307f60c8e0a`  
		Last Modified: Mon, 30 Oct 2023 23:50:44 GMT  
		Size: 18.9 MB (18858788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf992ac9f7594e95247c785c373702afa5ebbf20db8b34fad80efa1ff3e0736`  
		Last Modified: Mon, 30 Oct 2023 23:52:03 GMT  
		Size: 46.6 MB (46623965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652d455f0a073aa4bc59de2e451f4c5a2ad6d6d9cb13538ef955d11e722e6c45`  
		Last Modified: Mon, 30 Oct 2023 23:51:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce918b0b707b682534041104ace8701cb441f12b5ce2fb5e983bfe29694385`  
		Last Modified: Mon, 30 Oct 2023 23:51:58 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa512d8c7aada52b2d7bd906e3bae22e22f3025a7ed09a1f0adf9e2b9c7aaf6`  
		Last Modified: Tue, 31 Oct 2023 03:09:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ead55cfb97930802d78caa744029121af0f1f183f833ff3b343994e221908d2`  
		Last Modified: Tue, 31 Oct 2023 03:12:45 GMT  
		Size: 12.3 MB (12323885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b356d7f42ba8fdc9a6776a03e33f6a4064e2b480ae9437e7a91726fe33aede87`  
		Last Modified: Tue, 31 Oct 2023 03:12:45 GMT  
		Size: 2.8 MB (2812514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002231584dc0033a1da2dc9be37489f14ee3b13d0b655e81b5c5b422a8bf2bbd`  
		Last Modified: Tue, 31 Oct 2023 03:12:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e118aba5532091f9ab138a791f61e60f5ffaa5ebce1ace44c549fb6b8981cca1`  
		Last Modified: Thu, 09 Nov 2023 20:57:30 GMT  
		Size: 173.4 MB (173391884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f11ffe28bb16fb96aa091b2495b15080efb318aa51b99c8a06b05b44e4ece5`  
		Last Modified: Thu, 09 Nov 2023 20:57:27 GMT  
		Size: 309.1 MB (309079664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def6ca7fe20195766249d5eb00f64aa6f081fbf8fd343eafd9f31f446b1e19ca`  
		Last Modified: Thu, 09 Nov 2023 20:58:35 GMT  
		Size: 603.4 KB (603392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d52729d7e2b30db251417d519a87d90e35d82afd49586284ac991f5bda533`  
		Last Modified: Thu, 09 Nov 2023 20:58:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea612eae395fcd4001d6bdb7e927b95523531d7f16206d21316a0221fdefba`  
		Last Modified: Thu, 09 Nov 2023 20:58:34 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1f785b1febd6405a6eb97cc486fd545a35668492af9a93d41861567c4ccf83`  
		Last Modified: Thu, 09 Nov 2023 20:58:35 GMT  
		Size: 6.0 KB (6015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2666cc7e9642bc9b1f11f91f0005c3fca2a9b604bc3e3837d82f26bdeaf0f48`  
		Last Modified: Thu, 09 Nov 2023 20:58:34 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
