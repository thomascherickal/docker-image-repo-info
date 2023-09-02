## `xwiki:stable-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:0e4ed7a23e210ae801e1bf193b559a9536d90c18ebac746166ba731f0b3e40cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:79bb6a4e365295692d16ba806fabdba35627056a377e8fcf34721b6dc55827df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **591.1 MB (591113760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7618042ded8e81fce622229986c2c119ab2d56d9ec189a07fb8966eefe93629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:39:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 15:39:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 15:39:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 15:39:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Aug 2023 20:22:08 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Thu, 31 Aug 2023 20:23:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 31 Aug 2023 20:23:12 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 31 Aug 2023 20:23:12 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 31 Aug 2023 20:23:12 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 31 Aug 2023 22:29:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 31 Aug 2023 22:29:51 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 22:29:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 31 Aug 2023 22:29:51 GMT
WORKDIR /usr/local/tomcat
# Thu, 31 Aug 2023 22:29:51 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 31 Aug 2023 22:29:51 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 31 Aug 2023 22:32:51 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 31 Aug 2023 22:32:51 GMT
ENV TOMCAT_MAJOR=9
# Thu, 31 Aug 2023 22:32:51 GMT
ENV TOMCAT_VERSION=9.0.80
# Thu, 31 Aug 2023 22:32:51 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Thu, 31 Aug 2023 22:32:51 GMT
COPY dir:8732da32500112158bc197e9b7f498c8f335c2b13ed4db1d00b9568c9718b132 in /usr/local/tomcat 
# Thu, 31 Aug 2023 22:32:55 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Aug 2023 22:32:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 31 Aug 2023 22:32:56 GMT
EXPOSE 8080
# Thu, 31 Aug 2023 22:32:57 GMT
ENTRYPOINT []
# Thu, 31 Aug 2023 22:32:57 GMT
CMD ["catalina.sh" "run"]
# Fri, 01 Sep 2023 00:28:42 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 01 Sep 2023 00:28:42 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 01 Sep 2023 00:28:42 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 01 Sep 2023 00:28:43 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 01 Sep 2023 00:28:43 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 01 Sep 2023 00:28:43 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 01 Sep 2023 00:30:08 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 00:30:09 GMT
ENV XWIKI_VERSION=15.7
# Fri, 01 Sep 2023 00:30:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.7
# Fri, 01 Sep 2023 00:30:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=f4c725d1b5b184693cec0477910d0a238747265820aade23961d6578f7000b64
# Fri, 01 Sep 2023 00:30:50 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 01 Sep 2023 00:32:30 GMT
ENV MARIADB_JDBC_VERSION=3.2.0
# Fri, 01 Sep 2023 00:32:30 GMT
ENV MARIADB_JDBC_SHA256=adf9df10bc9b2a137def36d6a495812258f430d4a8f7946727c61558e6c73941
# Fri, 01 Sep 2023 00:32:30 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.2.0
# Fri, 01 Sep 2023 00:32:30 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.2.0.jar
# Fri, 01 Sep 2023 00:32:30 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.2.0.jar
# Fri, 01 Sep 2023 00:32:31 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Fri, 01 Sep 2023 00:32:31 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 01 Sep 2023 00:32:31 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 01 Sep 2023 00:32:32 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 01 Sep 2023 00:32:32 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 01 Sep 2023 00:32:32 GMT
VOLUME [/usr/local/xwiki]
# Fri, 01 Sep 2023 00:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Sep 2023 00:32:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabb03f19f5a305a4162b2dadb7942d094cb8ae82bfbb4ac13d4df822a60ffe3`  
		Last Modified: Wed, 16 Aug 2023 15:43:09 GMT  
		Size: 12.9 MB (12902780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48129c66e00fbeb066ade86c5989d0b1a47e82f72760a557edf1a9579917e115`  
		Last Modified: Thu, 31 Aug 2023 20:29:16 GMT  
		Size: 46.9 MB (46864354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676d95d9ec61b3f4081a3408ef7d451cebaaf6635293c6b4ac3435b4f106026`  
		Last Modified: Thu, 31 Aug 2023 20:29:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210b81b9d7fbce0801369da25bd01229b41d9af91a215c103a1b12e549e38f73`  
		Last Modified: Thu, 31 Aug 2023 20:29:10 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f28ca4058caae83938bc8ff5601404834db828e5e57cd2d30b1ef47428982`  
		Last Modified: Thu, 31 Aug 2023 22:41:13 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228041ae253e0bd4ff481f6d8a0d916f629f2f7b9d7c3ba2d3047fdfd6c7cf6e`  
		Last Modified: Thu, 31 Aug 2023 22:43:30 GMT  
		Size: 12.3 MB (12285229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d9957a6b80cf1ed0f03f75a8390d93d0964878caa71fb1ba936ebc625627b9`  
		Last Modified: Thu, 31 Aug 2023 22:43:29 GMT  
		Size: 455.6 KB (455605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6731a1970f51838a87872c1100a6a7d144d15c0b4ba8c43e375494d4e8889f`  
		Last Modified: Thu, 31 Aug 2023 22:43:29 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c23a6ca7dd465287cd81d341c71e2b36d43a21d61590451876c036cb54db583`  
		Last Modified: Fri, 01 Sep 2023 00:36:47 GMT  
		Size: 178.4 MB (178356773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466aac6b282539e231fac72f70c7bf25eb2aae07613d97d601e2f8c17108ba2d`  
		Last Modified: Fri, 01 Sep 2023 00:36:38 GMT  
		Size: 309.2 MB (309193993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d52341bae58ee31e5b389d34b9b0565ebde7b61b7f1bdaf0c2b5e81bb3bf98`  
		Last Modified: Fri, 01 Sep 2023 00:38:04 GMT  
		Size: 603.4 KB (603391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d8c5a6937c801bc527b7f65764a7527bb1df04b1a102aea6b04d4215a72019`  
		Last Modified: Fri, 01 Sep 2023 00:38:03 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5657d5e2ea51e0e3da348203e663a603f6488ead442a32d09b70c7b3075cc8ef`  
		Last Modified: Fri, 01 Sep 2023 00:38:03 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc0a3bb00401bdaa18eaaf20af22ab1d428e74b4c72e5d65a202609e76335e5`  
		Last Modified: Fri, 01 Sep 2023 00:38:03 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5a9da4c51d408dce5a3fef8abf3200bb76c0590988908060d4966315879e8d`  
		Last Modified: Fri, 01 Sep 2023 00:38:03 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:584d0d57f550b39fec1f9777fcb065f6f0006b466d2ed47b27f835b887eeb5e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.4 MB (582384339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b822ed463c5226977aaa57b847d9645de23ed35d73cb3a3251a0bf90e1692a5a`
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
# Sat, 02 Sep 2023 04:07:53 GMT
ENV XWIKI_VERSION=15.7
# Sat, 02 Sep 2023 04:07:53 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.7
# Sat, 02 Sep 2023 04:07:53 GMT
ENV XWIKI_DOWNLOAD_SHA256=f4c725d1b5b184693cec0477910d0a238747265820aade23961d6578f7000b64
# Sat, 02 Sep 2023 04:08:33 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 02 Sep 2023 04:10:12 GMT
ENV MARIADB_JDBC_VERSION=3.2.0
# Sat, 02 Sep 2023 04:10:12 GMT
ENV MARIADB_JDBC_SHA256=adf9df10bc9b2a137def36d6a495812258f430d4a8f7946727c61558e6c73941
# Sat, 02 Sep 2023 04:10:12 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.2.0
# Sat, 02 Sep 2023 04:10:12 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.2.0.jar
# Sat, 02 Sep 2023 04:10:12 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.2.0.jar
# Sat, 02 Sep 2023 04:10:13 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Sat, 02 Sep 2023 04:10:13 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 02 Sep 2023 04:10:13 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 02 Sep 2023 04:10:13 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 02 Sep 2023 04:10:13 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 02 Sep 2023 04:10:13 GMT
VOLUME [/usr/local/xwiki]
# Sat, 02 Sep 2023 04:10:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 Sep 2023 04:10:14 GMT
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
	-	`sha256:aa2e0e8013e76bfc8e1ccd20e4fb882868d4fd35e933a4202752607558826ec0`  
		Last Modified: Sat, 02 Sep 2023 04:14:23 GMT  
		Size: 309.2 MB (309194097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9da86aefa16e7f93b468d44b546e9a4d7bc6bfa2cd5c427de4a9945d45715f2`  
		Last Modified: Sat, 02 Sep 2023 04:15:33 GMT  
		Size: 603.4 KB (603392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5348bc3dbdf6eabe4cf6960df43a9e023aee0493d2de5cf047c882bf60586`  
		Last Modified: Sat, 02 Sep 2023 04:15:32 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bf83d68a2cfc60700558a5462abfd9b7b9358b07f934b8dd62abae13fe43d`  
		Last Modified: Sat, 02 Sep 2023 04:15:32 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3eb0adfee366efcb81a4e056864ab285f4ac45b4f8583ce7988a5cb65080c6`  
		Last Modified: Sat, 02 Sep 2023 04:15:32 GMT  
		Size: 6.3 KB (6310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a612a6f34673b6e80983a40601d47854d6b9ec9a407707cb5dce1be3ae38e44`  
		Last Modified: Sat, 02 Sep 2023 04:15:32 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
