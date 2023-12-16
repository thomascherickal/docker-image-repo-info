## `xwiki:latest`

```console
$ docker pull xwiki@sha256:272550395b7582a8631a0a7cfb393e9218b4126b737ca3294070bd48c500c9ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:latest` - linux; amd64

```console
$ docker pull xwiki@sha256:1818ccdb711b1c855894a11bfea06cd4a064cb3b762a7e7d8c5861f7d098e01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **595.5 MB (595515252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fad3df8469167dcd805fbc96356e14723490fb8fe734acef105de85d995463`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:16:13 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 16 Dec 2023 10:16:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Dec 2023 10:16:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Dec 2023 10:18:54 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:18:54 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 16 Dec 2023 10:19:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 16 Dec 2023 10:19:30 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 16 Dec 2023 10:19:30 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 16 Dec 2023 10:19:30 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 16 Dec 2023 16:07:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 16 Dec 2023 16:07:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Dec 2023 16:07:07 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 16 Dec 2023 16:07:07 GMT
WORKDIR /usr/local/tomcat
# Sat, 16 Dec 2023 16:07:07 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 16 Dec 2023 16:07:07 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 16 Dec 2023 16:09:32 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 16 Dec 2023 16:09:32 GMT
ENV TOMCAT_MAJOR=9
# Sat, 16 Dec 2023 16:09:32 GMT
ENV TOMCAT_VERSION=9.0.84
# Sat, 16 Dec 2023 16:09:32 GMT
ENV TOMCAT_SHA512=85a42ab5e7e4cb1923888e96a78a0f277a870d06e76147a95457878c124001c9a317eade4ad69c249a460ffe2cbefe894022b84389cdf33038bc456e3699c8e3
# Sat, 16 Dec 2023 16:09:32 GMT
COPY dir:e3a76c94a246a1206356fe923c85a36b030f13bc6f6e832187da5052d71cee0e in /usr/local/tomcat 
# Sat, 16 Dec 2023 16:09:36 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 16:09:38 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 16 Dec 2023 16:09:38 GMT
EXPOSE 8080
# Sat, 16 Dec 2023 16:09:38 GMT
ENTRYPOINT []
# Sat, 16 Dec 2023 16:09:38 GMT
CMD ["catalina.sh" "run"]
# Sat, 16 Dec 2023 19:41:04 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 16 Dec 2023 19:41:04 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 16 Dec 2023 19:41:04 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 16 Dec 2023 19:41:04 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 16 Dec 2023 19:41:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 16 Dec 2023 19:41:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 16 Dec 2023 19:42:34 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 19:42:36 GMT
ENV XWIKI_VERSION=15.10.1
# Sat, 16 Dec 2023 19:42:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.10.1
# Sat, 16 Dec 2023 19:42:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=a48057e5d82683e6f722be3868d8013b8e4d27d970b03309565a7f5a46f049f9
# Sat, 16 Dec 2023 19:43:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 16 Dec 2023 19:43:16 GMT
ENV MYSQL_JDBC_VERSION=8.2.0
# Sat, 16 Dec 2023 19:43:16 GMT
ENV MYSQL_JDBC_SHA256=06f14fbd664d0e382347489e66495ca27ab7e6c2e1d9969a496931736197465f
# Sat, 16 Dec 2023 19:43:16 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.2.0
# Sat, 16 Dec 2023 19:43:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.2.0.jar
# Sat, 16 Dec 2023 19:43:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.2.0.jar
# Sat, 16 Dec 2023 19:43:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Sat, 16 Dec 2023 19:43:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 16 Dec 2023 19:43:18 GMT
COPY file:5f2a4ed869db1db1cb3a7b1d056ce086793eaabda6970493836040aa3d66ed8a in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 16 Dec 2023 19:43:18 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 16 Dec 2023 19:43:18 GMT
COPY file:b4aa3ce54fbec701991ab2ba0888227771ac09202a9e4ba777edbd49ed958e27 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 16 Dec 2023 19:43:18 GMT
VOLUME [/usr/local/xwiki]
# Sat, 16 Dec 2023 19:43:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Dec 2023 19:43:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f838805bddf9c7d83f7f51716a77602920f9057ade57b344c071481b5214767`  
		Last Modified: Sat, 16 Dec 2023 10:23:47 GMT  
		Size: 17.5 MB (17456128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eee5bc80e633b7f89402fb78469504f2d0662c7c827954ff259867d024278b`  
		Last Modified: Sat, 16 Dec 2023 10:24:28 GMT  
		Size: 47.1 MB (47149325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51526e7965d895bb7535ad46133791589d87f78882f553e5e63f8aed0568dabd`  
		Last Modified: Sat, 16 Dec 2023 10:24:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcdc7c6c1603bef17eec1b194fd954703a005aff5db2d15302f85b01b494351`  
		Last Modified: Sat, 16 Dec 2023 10:24:21 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81f1b04d3d203216bfcc90d5a6429b5c33ec66e790e3ebf566431088f5212c`  
		Last Modified: Sat, 16 Dec 2023 16:24:58 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a603ca3ebf9e8f0eb997467ce50ef8dfd4e49196308c1a39f9c5c0c39d2846b`  
		Last Modified: Sat, 16 Dec 2023 16:27:49 GMT  
		Size: 12.4 MB (12398194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b70543ac62867c34368428a8432713e13dbcb451521adfe0879fc51c5cae2e`  
		Last Modified: Sat, 16 Dec 2023 16:27:48 GMT  
		Size: 458.4 KB (458432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a684fd03abd5ec4c3528f0458050f8b03af9c5a885783d748df8617d90250c6`  
		Last Modified: Sat, 16 Dec 2023 16:27:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662430d7fcc4a693daf59b478f6610856c0218eedea85e938eae7f66ab214115`  
		Last Modified: Sat, 16 Dec 2023 19:49:10 GMT  
		Size: 178.4 MB (178366838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1737e384b4e93718d70122429436341cb255d26588518fb9d9f4e23a5a6b0067`  
		Last Modified: Sat, 16 Dec 2023 19:49:03 GMT  
		Size: 306.9 MB (306874995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb604e7de8534d5b44cd80352fe8aa882a24251b72dc4774819ad1e434a00ac1`  
		Last Modified: Sat, 16 Dec 2023 19:48:46 GMT  
		Size: 2.4 MB (2350948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478ae1668f55e7b1ba9b6505fe47aede5ce734d253ac6ea9d4bc22962942bf96`  
		Last Modified: Sat, 16 Dec 2023 19:48:46 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d58c77d3fb20afde8ef158c2374d4ed17b0e26036d12f3f598d43c27e1f34bc`  
		Last Modified: Sat, 16 Dec 2023 19:48:46 GMT  
		Size: 2.4 KB (2374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9502fd967b7b4d6ed5d5376d9cb437d1eab37195787f78fa4f2342daf57101d`  
		Last Modified: Sat, 16 Dec 2023 19:48:46 GMT  
		Size: 6.4 KB (6417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083c9a6fb662da117865e6499bfa9c14fa8a18c8e72eab5128e4171ebc4c6b07`  
		Last Modified: Sat, 16 Dec 2023 19:48:46 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:latest` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:f18251cd17736ec9170f808fd8b1bb2804f5ffeb94eb03611edc4bf38a74218d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **589.4 MB (589393889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ec94881d9672f6d72ca5693612aefc82a5b1e069d56eedb56e492a7a2661e08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:02:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 16 Dec 2023 10:02:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Dec 2023 10:02:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Dec 2023 10:04:31 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         binutils         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:04:32 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Sat, 16 Dec 2023 10:04:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='05b192f81ed478178ba953a2a779b67fc5a810acadb633ad69f8c4412399edb8';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.9_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c37f729200b572884b8f8e157852c739be728d61d9a1da0f920104876d324733';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_x64_linux_hotspot_17.0.9_9.tar.gz';          ;;        armhf|arm)          ESUM='5ae1f8cae358e41083a6b44f53c6f0daeb657f83c293da6c8733f68278e13703';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_arm_linux_hotspot_17.0.9_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79c85ecf1320c67b828310167e1ced62e402bc86a5d47ca9cc7bfa3b708cb07a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.9_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c4f2249bee785aa8c754741aa24d035e02b4e6d844e35b2b20030374d8fbab75';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9/OpenJDK17U-jre_s390x_linux_hotspot_17.0.9_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 16 Dec 2023 10:04:57 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Sat, 16 Dec 2023 10:04:57 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 16 Dec 2023 10:04:57 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 16 Dec 2023 14:58:15 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 16 Dec 2023 14:58:15 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Dec 2023 14:58:16 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 16 Dec 2023 14:58:16 GMT
WORKDIR /usr/local/tomcat
# Sat, 16 Dec 2023 14:58:16 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 16 Dec 2023 14:58:16 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 16 Dec 2023 15:00:13 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 16 Dec 2023 15:00:13 GMT
ENV TOMCAT_MAJOR=9
# Sat, 16 Dec 2023 15:00:13 GMT
ENV TOMCAT_VERSION=9.0.84
# Sat, 16 Dec 2023 15:00:13 GMT
ENV TOMCAT_SHA512=85a42ab5e7e4cb1923888e96a78a0f277a870d06e76147a95457878c124001c9a317eade4ad69c249a460ffe2cbefe894022b84389cdf33038bc456e3699c8e3
# Sat, 16 Dec 2023 15:00:13 GMT
COPY dir:14fe7e4b8e31f53a38fe02615c860260f06f1bfa5d55349e5c610bb0eaaf3673 in /usr/local/tomcat 
# Sat, 16 Dec 2023 15:00:17 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 15:00:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 16 Dec 2023 15:00:18 GMT
EXPOSE 8080
# Sat, 16 Dec 2023 15:00:18 GMT
ENTRYPOINT []
# Sat, 16 Dec 2023 15:00:18 GMT
CMD ["catalina.sh" "run"]
# Sat, 16 Dec 2023 18:02:27 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 16 Dec 2023 18:02:27 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 16 Dec 2023 18:02:27 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 16 Dec 2023 18:02:27 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 16 Dec 2023 18:02:27 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 16 Dec 2023 18:02:27 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 16 Dec 2023 18:04:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 18:04:20 GMT
ENV XWIKI_VERSION=15.10.1
# Sat, 16 Dec 2023 18:04:20 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.10.1
# Sat, 16 Dec 2023 18:04:20 GMT
ENV XWIKI_DOWNLOAD_SHA256=a48057e5d82683e6f722be3868d8013b8e4d27d970b03309565a7f5a46f049f9
# Sat, 16 Dec 2023 18:04:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 16 Dec 2023 18:05:02 GMT
ENV MYSQL_JDBC_VERSION=8.2.0
# Sat, 16 Dec 2023 18:05:02 GMT
ENV MYSQL_JDBC_SHA256=06f14fbd664d0e382347489e66495ca27ab7e6c2e1d9969a496931736197465f
# Sat, 16 Dec 2023 18:05:02 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.2.0
# Sat, 16 Dec 2023 18:05:02 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.2.0.jar
# Sat, 16 Dec 2023 18:05:02 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.2.0.jar
# Sat, 16 Dec 2023 18:05:03 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Sat, 16 Dec 2023 18:05:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 16 Dec 2023 18:05:03 GMT
COPY file:5f2a4ed869db1db1cb3a7b1d056ce086793eaabda6970493836040aa3d66ed8a in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 16 Dec 2023 18:05:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 16 Dec 2023 18:05:03 GMT
COPY file:b4aa3ce54fbec701991ab2ba0888227771ac09202a9e4ba777edbd49ed958e27 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 16 Dec 2023 18:05:04 GMT
VOLUME [/usr/local/xwiki]
# Sat, 16 Dec 2023 18:05:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Dec 2023 18:05:04 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83d9c33e24ca521e40939a701f20c41285b4488136968b6007b00f5ea0e1267`  
		Last Modified: Sat, 16 Dec 2023 10:08:54 GMT  
		Size: 18.9 MB (18857814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced1602447389bf6ad2464c27ffc94e85095dbfdb47f78a2096081e80388ad97`  
		Last Modified: Sat, 16 Dec 2023 10:09:35 GMT  
		Size: 46.6 MB (46624027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6457113e3d5d5e26e07af4b78a197170e362a87e9acf2597817bf8e41b61b864`  
		Last Modified: Sat, 16 Dec 2023 10:09:30 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764df9f717c8b617f5bd26b1b7a44dfb44e89d4a1bc26be0eb4a08d0696d3e49`  
		Last Modified: Sat, 16 Dec 2023 10:09:30 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fdc1608413c55e6f71ba5c11e8a186c5cdf1ffd462d135094650174976fd36`  
		Last Modified: Sat, 16 Dec 2023 15:13:29 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040f9b1d3ea5ed9193ca2803556daa46af53b68c910758193f72f2d9ea7583f6`  
		Last Modified: Sat, 16 Dec 2023 15:16:19 GMT  
		Size: 12.4 MB (12407499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b105fa48bd69dab1ec528eb0a9cdaf37f46e8af363a642b3f44e619e7751d4ed`  
		Last Modified: Sat, 16 Dec 2023 15:16:18 GMT  
		Size: 458.5 KB (458463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b656c2cf87b11b1a6165fa929daa3b987a92d55dd64f4151810c4a9d3ee4cd8`  
		Last Modified: Sat, 16 Dec 2023 15:16:18 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f60916f51a359375337649cb777dd0f742039aedb8e4329c32e9517494eae79`  
		Last Modified: Sat, 16 Dec 2023 18:10:48 GMT  
		Size: 173.4 MB (173406076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab679cf684e85744aad2b2e08aff9727a2f3a34d0555e17d0db9f8e95302b7`  
		Last Modified: Sat, 16 Dec 2023 18:10:45 GMT  
		Size: 306.9 MB (306874961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e16b08259631f61117427ddcd091f77109c01a6873e1b8d066c24a9a597afe`  
		Last Modified: Sat, 16 Dec 2023 18:10:31 GMT  
		Size: 2.4 MB (2350959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1720ea1986a291aca860bec3a16366287931c06cdc4822c3af42c4b30febbd1e`  
		Last Modified: Sat, 16 Dec 2023 18:10:31 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556af578769e58f1e4627c2c842ae1bda4008b871842f4b0fa223c791e66625e`  
		Last Modified: Sat, 16 Dec 2023 18:10:31 GMT  
		Size: 2.4 KB (2370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6f02ab65335b04fa15c1d010fa58e88546c285fb87d343ec89ff00e2ca58e9`  
		Last Modified: Sat, 16 Dec 2023 18:10:31 GMT  
		Size: 6.4 KB (6413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc8ce3d9f0feb9ded4215ba585e3f4f805323dfbb3dcda487a0468adc39419`  
		Last Modified: Sat, 16 Dec 2023 18:10:31 GMT  
		Size: 2.5 KB (2483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
